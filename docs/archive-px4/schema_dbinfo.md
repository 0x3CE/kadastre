_──────────────────────┬─────────────┬────────────────────────────────────────┬───┬────────────┬────────┬─────────────────┐
│      column_name      │ column_type │                  min                   │ … │    q75     │ count  │ null_percentage │
│        varchar        │   varchar   │                varchar                 │ … │  varchar   │ int64  │  decimal(9,2)   │
├───────────────────────┼─────────────┼────────────────────────────────────────┼───┼────────────┼────────┼─────────────────┤
│ log_id                │ UUID        │ 00003ade-ba96-4f19-bfad-7c731d7a8f7b   │ … │ NULL       │ 488002 │            0.00 │
│ log_date              │ DATE        │ 2016-12-09                             │ … │ 2026-04-02 │ 488002 │            0.00 │
│ description           │ VARCHAR     │                                        │ … │ NULL       │ 488002 │            0.00 │
│ feedback              │ VARCHAR     │                                        │ … │ NULL       │ 488002 │            0.00 │
│ type                  │ VARCHAR     │ flightreport                           │ … │ NULL       │ 488002 │            0.00 │
│ wind_speed            │ HUGEINT     │ -1                                     │ … │ -1         │ 488002 │            0.00 │
│ rating                │ VARCHAR     │                                        │ … │ NULL       │ 488002 │            0.00 │
│ video_url             │ VARCHAR     │                                        │ … │ NULL       │ 488002 │            0.00 │
│ error_labels          │ BIGINT[]    │ []                                     │ … │ NULL       │ 488002 │            0.00 │
│ source                │ VARCHAR     │ PX4 Flycore PR validation              │ … │ NULL       │ 488002 │            0.00 │
│ duration_s            │ BIGINT      │ 0                                      │ … │ 211        │ 488002 │            0.00 │
│ mav_type              │ VARCHAR     │ Airship, controlled                    │ … │ NULL       │ 488002 │            0.00 │
│ estimator             │ VARCHAR     │ EKF2                                   │ … │ NULL       │ 488002 │            0.00 │
│ sys_autostart_id      │ BIGINT      │ 0                                      │ … │ 6001       │ 488002 │            0.00 │
│ sys_hw                │ VARCHAR     │                                        │ … │ NULL       │ 488002 │            0.00 │
│ ver_sw                │ VARCHAR     │                                        │ … │ NULL       │ 488002 │            0.00 │
│ ver_sw_release        │ VARCHAR     │                                        │ … │ NULL       │ 488002 │            0.00 │
│ num_logged_errors     │ BIGINT      │ 0                                      │ … │ 0          │ 488002 │            0.00 │
│ num_logged_warnings   │ BIGINT      │ 0                                      │ … │ 5          │ 488002 │            0.00 │
│ flight_modes          │ BIGINT[]    │ []                                     │ … │ NULL       │ 488002 │            0.00 │
│ vehicle_uuid          │ VARCHAR     │                                        │ … │ NULL       │ 488002 │            0.00 │
│ flight_mode_durations │ BIGINT[][]  │ []                                     │ … │ NULL       │ 488002 │            0.00 │
│ vehicle_name          │ VARCHAR     │                                        │ … │ NULL       │ 488002 │            0.00 │
│ airframe_name         │ VARCHAR     │                                        │ … │ NULL       │ 488002 │            0.00 │
│ airframe_type         │ JSON        │ "Airship"                              │ … │ NULL       │ 488002 │            0.00 │
│ download_url          │ VARCHAR     │ https://cdn.logs.px4.io/00003ade-ba96… │ … │ NULL       │ 488002 │            0.00 │
└───────────────────────┴─────────────┴────────────────────────────────────────┴───┴────────────┴────────┴─────────────────┘