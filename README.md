# single-stage-pipeline-reg
Single stage pipeline register with valid/ready handshake in SystemVerilog
# Single Stage Pipeline Register

This repository contains a fully synthesizable SystemVerilog implementation of a single-stage pipeline register using a standard valid/ready handshake.

## Features
- Supports backpressure without data loss or duplication
- Clean reset to empty state
- Fully synthesizable RTL
- Bubble-free data transfer

## Interface
- Input: in_valid, in_ready, in_data
- Output: out_valid, out_ready, out_data

## Description
The module accepts input data when both in_valid and in_ready are asserted. Data is stored internally and presented on the output interface. Backpressure from downstream is correctly handled using the ready/valid protocol.

## Language
- SystemVerilog

## Author
- Niharika Veggalam
