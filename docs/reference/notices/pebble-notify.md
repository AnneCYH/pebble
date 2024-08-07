# Pebble notify command

The notify command records a custom notice with the specified key and optional data fields.

## Usage

```{terminal}
   :input: pebble notify --help
Usage:
  pebble notify [notify-OPTIONS] <key> [<name=value>...]

The notify command records a custom notice with the specified key and optional
data fields.

[notify command options]
      --repeat-after=   Prevent notice with same type and key from reoccurring within this duration
```

## Examples

To record `custom` notices, use `pebble notify` -- the notice user ID will be set to the client's user ID:

```{terminal}
   :input: pebble notify example.com/foo
Recorded notice 1
```

Notify with two data fields:

```{terminal}
   :input: pebble notify other.com/bar name=value email=john@smith.com  
Recorded notice 2
```
