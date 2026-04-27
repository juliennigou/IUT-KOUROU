# HDFS Preprocessed Dataset

This folder contains the preprocessed HDFS data used for anomaly detection exercises.

For student work, use:

- [HDFS_ml_dataset_student.csv](/Users/juliennigou/iut-kourou/Project/HDFS_v1/preprocessed/HDFS_ml_dataset_student.csv)

## What is in the student CSV?

Each row represents one HDFS block trace identified by a `BlockId`.

The file contains:

- `BlockId`: unique identifier of the block trace
- `AnomalyLabel`: target label with two values
  - `Normal`
  - `Anomaly`
- `E1` to `E29`: event occurrence counts for that block trace

That means each `E` column tells you how many times a given log event appeared for that block.

## Shape of the file

- Rows: `575,061`
- Columns: `31`
- Target column: `AnomalyLabel`
- Feature columns: `E1` to `E29`

## How to use it

Typical ML workflow:

1. Load `HDFS_ml_dataset_student.csv`
2. Keep `E1` to `E29` as input features
3. Convert `AnomalyLabel` into a numeric target yourself
  - for example: `Normal = 0`, `Anomaly = 1`
4. Decide whether to keep or drop `BlockId`

In most ML models, `BlockId` should be treated as an identifier and not as a predictive feature.

## Meaning of the event columns

The exact event-template mapping comes from [HDFS.log_templates.csv](/Users/juliennigou/iut-kourou/Project/HDFS_v1/preprocessed/HDFS.log_templates.csv).

Here is the mapping used in the dataset:

- `E1`: Adding an already existing block
- `E2`: Verification succeeded for a block
- `E3`: Served block to a client
- `E4`: Exception while serving a block to a client
- `E5`: Receiving block from source to destination
- `E6`: Received block from source to destination
- `E7`: `writeBlock` received exception
- `E8`: `PacketResponder` interrupted for a block
- `E9`: Received block of a given size from a source
- `E10`: `PacketResponder` exception
- `E11`: `PacketResponder` terminating for a block
- `E12`: Exception writing block to mirror
- `E13`: Receiving empty packet for a block
- `E14`: Exception in `receiveBlock`
- `E15`: Changing block file offset
- `E16`: Transmitted block to another node
- `E17`: Failed to transfer a block
- `E18`: Starting thread to transfer a block
- `E19`: Reopen block
- `E20`: Unexpected error while deleting a block, `BlockInfo` not found in `volumeMap`
- `E21`: Deleting block file
- `E22`: `NameSystem allocateBlock`
- `E23`: Block delete added to `invalidSet`
- `E24`: Removing block from needed replications
- `E25`: Ask a node to replicate a block
- `E26`: `addStoredBlock` updated block map
- `E27`: Redundant `addStoredBlock` request received
- `E28`: `addStoredBlock` request for a block that does not belong to any file
- `E29`: `PendingReplicationMonitor` timed out a block

## Example

If a row contains:

- `E3 = 203`
- `E20 = 1`
- `E21 = 3`
- `E23 = 3`

it means that block was served many times, then later involved in deletion activity, and also had one unexpected delete-time error.

## files in this folder

- `Event_traces.csv`: event sequences and timing information per block
- `HDFS_ml_dataset.csv`: merged version with extra metadata columns

