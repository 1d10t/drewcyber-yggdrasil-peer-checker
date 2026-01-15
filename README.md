# peer_checker.go
Yggdrasil [peers](https://github.com/yggdrasil-network/public-peers) checker. 

Script https://github.com/zhoreeq/peer_checker.py rewritten using Golang.

Usage:
```
go run . ../public-peers/
```

or
```
go build
./peer_checker ../public-peers
```

or export first 10 fastest alive peers in JSON format
```
go run . --json ~/public-peers/  | jq '.alive[:10] | map(.uri)'
```
