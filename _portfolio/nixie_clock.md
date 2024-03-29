---
title: "Nixie radio clock"
excerpt: "Design and construction of a radio clock based around vintage Nixie tubes <br/><img src='/images/500x300.png'>"
collection: portfolio
---

One of the most famous projects in the maker community is the Nixie clock, based on one of the many models of the vintage Nixie tubes.
The display of choice were the IN-12, compact and cheap with respect to the other models available.

## High voltage power supply
Nixie tubes are essentially a type of discharge lamp, so they require a high voltage to operate, 170V DC to strike and 160V to maintain the light.
A high voltage power supply is needed, and since a low budget is the priority in this project given the high cost of the tubes i decided to build it discreetly.
A simple design found online based around the NE555 chip is perfect for the job, configured as a switching power supply it manages to step up 9V to 170V DC with a margin for regulation. It can supply easily the 2mA per tube at 160V so it's at least 1W capable.

## Nixie tubes PCB
Once the power supply is done i tested the tubes to see if they all worked and thankfully they did, with a beautiful and uniform orange glow.

Given the non standard pitch of the pins of tubes i couldn't use a prototype board to wire them together (wiring them pin by pin with wire  to a protoboard is not an ideal choice given the frustration it could cause if done wrong).
This problem gave me the opportunity to finally print a circuit board at home and use the ferric cloride i had for years sitting on the shelf.
Once i designed, printed, and transfered the circuit on the board i proceeded to etch the copper with a ferric cloride solution. The etch turned out very well defined, with even the smallest traces being etched without problems.

The next step required to drill all the holes for the tubes and the connector; i had to build a jig to use a cheap dremel to drill the through holes but i managed to not destroy the board, so then i needed some sort of sockets for the tubes, to not stress them too much by soldering them directly to the PCB.

## High votage multiplexing

## Digital section of the circuit
