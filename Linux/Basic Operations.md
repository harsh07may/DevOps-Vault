**I/O Redirection (using < or >)**
- `command < [filename]`: Read Input from file.
- `command > [filename]`: Write Output to file (`>>` to append).

**Command Combinations (using pipes '|')**
`command1 | command2 | command3` : We can use 

 ```bash
 # Finding and modifying
 # (Finds log files older than 7 days and deletes them)
find . -name '*.log' -type f -mtime +7 -exec rm -f {} \;

# **Filtering output
# (Lists files and filters the output to only show lines containing "myFile")
ls -l | grep 'myFile'

# Chaining Operations
# (Displays error messages, sorts them, and shows unique errors with counts).
cat error.log | grep 'failed' | sort | uniq -c
```

**System Administration**
```bash
# Monitoring disk usage with filtering:
# Finds the top 10 largest directories within '/var'.
du -sh /var/* | sort -rh | head -n 10
```

**Quick hacks**: 
```bash
curl https://www.example.com > original.txt 
sleep 60 # Wait for a minute 
curl https://www.example.com > updated.txt 
diff original.txt updated.txt
```

```bash
# Find files over 100MB and compress them
find / -type f -size +100M -exec gzip {} \; 
```