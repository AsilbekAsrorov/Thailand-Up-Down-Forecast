# Dataset Information

## Source
Thailand street pedestrian tracking dataset collected via camera sensors.

## Sample file
`sample_dataset.csv` — 100,000 rows sampled from the full dataset.

## Columns
- `timestamp` — date and time of the tracking event
- `object_class` — type of object detected (e.g. person, vehicle)
- `direction` — movement direction of the detected object

## Target variables (created during preprocessing)
- `up_count` — number of people moving up per hour
- `down_count` — number of people moving down per hour

## Notes
The raw data is event-level (one row per detection).
The notebook aggregates it into hourly counts before modeling.