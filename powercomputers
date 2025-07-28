#!/bin/bash

if [[ $# -ne 1 || ! -f "$1" ]]; then
    echo "Command sample: Get-DomainComputer -Properties name,operatingsystem"
    echo "Usage: $0 <input_file>"
    exit 1
fi

declare -A host_os
declare -A host_os_key

while IFS= read -r line; do
    if [[ "$line" =~ ^name ]]; then
        host=$(echo "$line" | awk -F ': *' '{print $2}')
    elif [[ "$line" =~ ^operatingsystem ]]; then
        os=$(echo "$line" | awk -F ': *' '{print $2}')
        host_os["$host"]="$os"
        host_os_key["$host"]="$os"
    fi
done < "$1"

for host in "${!host_os[@]}"; do
    echo -e "${host_os_key[$host]}\t$host -> ${host_os[$host]}"
done | sort | cut -f2-
