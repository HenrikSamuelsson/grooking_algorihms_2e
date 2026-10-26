# Exercise 2.2 — Restaurant Order Queue

## Introduction

Solution to Exercise 2.2 from *Grokking Algorithms, Second Edition*.

## Problem

The problem statement is omitted due to copyright. See Exercise 2.2 in the referenced book.

## Solution

A valid choice is to use a linked list for the order queue. New orders are added to the back, and chefs take the first order from the front. A linked list can handle these insertions and deletions efficiently, and the app does not need random access to the orders.

A fixed-size array could also be a reasonable choice if the maximum queue size is known. A circular buffer would let the app add orders at the back and remove them from the front without shifting the remaining orders. The app would need to handle the queue becoming full like to roll over to the start and track the start and end indexes.

## Answer

linked list

## References

Bhargava, A. Y. (2024). *Grokking algorithms: An illustrated guide for programmers and other curious people* (2nd ed.). Manning Publications.

[← Previous](../exercise_02_01/exercise_02_01.md) | [Home](../../README.md) | [Next →](../exercise_02_03/exercise_02_03.md)