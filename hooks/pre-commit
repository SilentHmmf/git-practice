#!/bin/bash

repo_path=$(git rev-parse --show-toplevel)

txt_files=$(find "$repo_path" -type f -name "*.txt")
for file in $txt_files; do
    if ! grep -q "определенный_формат" "$file"; then
        echo "Файл $file не соответствует формату"
        exit 1
    fi
done
