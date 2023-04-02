#!/bin/bash

log_file="$1"

# Count 4xx and 5xx responses
count=$(grep -E "HTTP/1.[01]\" (4|5)[0-9][0-9]" "$log_file" | wc -l)

# If the cumulative number of errors exceeds 100, send an email alert
if [[ $count -gt 100 ]]; then
    echo "High number of error responses in $log_file: $count" | mail -s "Apache Error Alert" admin@example.com
fi
