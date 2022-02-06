# kpause

A shell script, to temporarily scale down namespaces and scale back as set before. E.g. to avoid restarting pods when the whole cluster will be shut down.

## Usage

    Usage:
             Pause:
             kpause [-n namespaces] [-v]
             Resume:
             kpause -r [-n namespaces] [-a] [-v]
    
    -h --help         print help
    -n --namespaces   operate on comma/space separated namespcaes, otheriwse only configured default namespace
    -v --verbose      debugging output
    -a --all          all namespaces, only valid for resume
    -r --resume       resume pods with previous scale

