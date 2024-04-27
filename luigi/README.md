# Luigi w/ kubernetes

## example

```bash
kind create cluster
```

```bash
poetry run luigi --module luigik8s.scripts.main PerlPi2 --local-scheduler
```