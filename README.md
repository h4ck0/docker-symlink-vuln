```

  % ./run_read.sh &>/dev/null & ; sleep 10s ; pkill -9 run.sh
  % chmod 0644 ex*/out # to fix up permissions for grep
  % grep 'SUCCESS' ex*/out | wc -l # managed to get it from the host
  2
  % grep 'FAILED'  ex*/out | wc -l # got the file from the container
  334
```
