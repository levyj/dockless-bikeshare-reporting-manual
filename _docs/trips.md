---
title: Trips
category: Monthly Submission
order: 1
---

## Scope

All Trips completed during the reporting period.  Trips in progress at the end of the reporting period should be held for the next report.  For the purposes of this file, a trip is a transaction with a single rider.

## File Format

Trip data must be reported using the following schema and reported with the following `[company]-trips-[date].csv`.

| Field | Element        | Data Type           | Required | Description                                                                                       |
|  T1   | Trip ID        | String              |   Yes    | A unique identifier that identifies the trip. The identifier should be permanently unique, not just within the reporting period.                                                    |
|  T2   | Bike ID        | String              |   Yes    | A unique identifier for the bicycle. Should be the same ID used throughout reporting requirements.|
|  T3   | Start Time     | ISO 8601 timestamp  |   Yes    | The date and time that the trip began.                                                            |
|  T4   | End Time       | ISO 8601 timestamp  |   Yes    | The date and time that the trip concluded.                                                        |
|  T5   | From Latitude  | Latitude (WGS83)    |   Yes    | Latitude of where the trip began.                                                                 |
|  T6   | From Longitude | Longitude (WGS83)   |   Yes    | Longitude of where the trip began.                                                                |
|  T7   | To Latitude    | Latitude (WGS83)    |   Yes    | Latitude of where the trip ended.                                                                 |
|  T8   | To Longitude   | Longitude (WGS83)   |   Yes    | Longitude of where the trip ended.                                                                |
|  T9   | Trip Distance  | Numeric (feet)      |   Yes    | The amount of distance the bicycle traveled during the course of the trip.                        |


