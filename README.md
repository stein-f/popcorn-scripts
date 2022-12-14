# popcorn-scripts

Hacky scripts to parse popcorn lounge transactions and output stats

# Prerequisites

The script depends on Golang being installed on your machine. You can install from here: https://go.dev/dl/

# Scripts

## Print world cup winners table

`go run scripts/winners-table/main.go`

Output

```text
W-L-P
9-2-1, shrimp: 1950     4FBNL...IW6D4
6-5-1, shrimp: 3600     chrundle.algo
6-5-1, shrimp: 3600     AI7QM...PGYX4
```

## Count bets on teams

`go run scripts/bets/main.go`

Output

```text
Germany: 35
Japan: 17
Over: 22
Under: 20
```

## Display bets for a given user

`go run scripts/show-wallet-bets/main.go`

Output

```text
Game: Senegal (+1) vs Netherlands (-1), Bet: Netherlands, Amount: 100
Game: Senegal vs Netherlands, Bet: Under 2.5 Goals, Amount: 300
Game: England (-1.5) vs Iran (+1.5), Bet: England, Amount: 300
Game: England vs Iran, Bet: Under 2.5 Goals, Amount: 300
```

# Run tests

```bash
make test
```
