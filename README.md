# Unveiling-the-Unseen-Video-Recognition-Attacks-in-Complex-Network-Environments-and-Playback-Modes

# GitHub Repository Description

## Introduction
This repository contains the code for the paper "Unveiling the Unseen: Video Recognition Attacks in Complex Network Environments and Playback Modes". As the content of this paper involves sniffing attacks, to prevent misuse, we have limited the functionality of the open-source program.

## Program and Dataset
We only provide executable programs and restrict the dataset to data prior to March 2024, providing only five traffic cases under four conditions. The program is divided into Windows and Linux versions. `data.cfg` contains the configuration related to file paths; `twitter` is the program for restoring video segment lengths, `make_db` is the program for building the database, and `match_mul_db` is the recognition program.

## Dataset
The dataset is too large, so it is placed in the release version. The `twitter_fingerprint_current.csv` in the `data` folder is the fingerprint of the video corresponding to 20 video streams, and `twitter_fingerprint_large-sal.csv` is the fingerprint of 302,358 videos. The folders are divided into `under a fluctuating network environment with seeking playback`, `under a fluctuating network environment with sequential playback`, `under a stable network environment with seeking playback`, `under a stable network environment with sequential playback`, and `all` folder containing the above four cases.

## Program Execution Flow
The program execution flow is to first execute `twitter` to generate the length of the restored video segment, then use `make_db` to generate the fingerprint library, and finally use `match_mul_db` for fingerprint recognition. The recognition result is displayed in `0_mul_DB_match`.

## Experimental Environment
The experimental environment of this paper's program is win11 (16GB memory) and Ubuntu22.04 (16GB memory).
