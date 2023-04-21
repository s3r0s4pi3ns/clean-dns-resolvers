# DNS servers

A list of public DNS servers is validated twice a day and saved into the file `resolvers.txt`. These sanitized DNS servers provide us with better & faster results, and we can avoid false positives or DNS servers that have been poisoned and reply with incorrect information

# Usage

## [PureDNS](https://github.com/d3mondev/puredns)

```bash
puredns resolve "subdomains_to_resolve.txt" -r "resolvers.txt" --resolvers-trusted "resolvers-trusted.txt" --write "valid_domains.txt"
```

## [ShuffleDNS](https://github.com/projectdiscovery/shuffledns)

```bash
shuffledns-list -silent -l "subdomains_to_resolve.txt" -r "resolvers.txt" -o "valid_domains.txt"
```
