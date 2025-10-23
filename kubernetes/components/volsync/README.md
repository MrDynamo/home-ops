# Volsync

## Replication Sources

| Workload    | Size | Volsync Replication Schedule | Crontab (UTC)   | Crontab (CST -5)   | Crontab (CDT -6)   |
|-------------|------|------------------------------|-----------------|--------------------|--------------------|
| bazarr      | 1Gi  | Wednesday @ 10:00            | `0 10 * * 3`    | `0 15 * * 3`       | `0 16 * * 3`       |
| dispatcharr | 1Gi  | Friday @ 10:00               | `0 10 * * 5`    | `0 15 * * 5`       | `0 16 * * 5`       |
| homepage    | 1Gi  | Thursday @ 04:00             | `0 4 * * 4`     | `0 9 * * 4`        | `0 10 * * 4`       |
| kometa      | 6Gi  | Thursday @ 05:00             | `0 5 * * 4`     | `0 10 * * 4`       | `0 11 * * 4`       |
| maintainerr | 1Gi  | Tuesday @ 08:00              | `0 8 * * 2`     | `0 13 * * 2`       | `0 14 * * 2`       |
| mealie      | 1Gi  | Thursday @ 06:00             | `0 6 * * 4`     | `0 11 * * 4`       | `0 12 * * 4`       |
| plex        | 18Gi | Monday @ 07:00               | `0 7 * * 1`     | `0 12 * * 1`       | `0 13 * * 1`       |
| prowlarr    | 1Gi  | Thursday @ 07:00             | `0 7 * * 4`     | `0 12 * * 4`       | `0 13 * * 4`       |
| radarr      | 2Gi  | Wednesday @ 08:00            | `0 8 * * 3`     | `0 13 * * 3`       | `0 14 * * 3`       |
| sabnzbd     | 1Gi  | Tuesday @ 06:00              | `0 6 * * 2`     | `0 11 * * 2`       | `0 12 * * 2`       |
| seerr       | 1Gi  | Tuesday @ 04:00              | `0 4 * * 2`     | `0 9 * * 2`        | `0 10 * * 2`       |
| sonarr      | 4Gi  | Wednesday @ 04:00            | `0 4 * * 3`     | `0 9 * * 3`        | `0 10 * * 3`       |
| tautulli    | 4Gi  | Friday @ 04:00               | `0 4 * * 5`     | `0 9 * * 5`        | `0 10 * * 5`       |
| wizarr      | 1Gi  | Friday @ 08:00               | `0 8 * * 5`     | `0 13 * * 5`       | `0 14 * * 5`       |
