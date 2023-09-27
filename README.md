# Aiken vesting contract

How to run this project:

Step 1: Download dependencies

```
aiken check
```

Step 2:  Build contract

```
aiken build
```

Step 3: Generate private keys and addresses for owner and beneficiary using Lucid

```
deno run --allow-net --allow-write generate-credentials.ts
```

Step 4: Run lock scripts
```
deno run --allow-net --allow-read --allow-env vesting_lock.ts <LOCK_UNTIL_IN_UNIX_TIME>
```

Step 5: Run unlocking scripts
```
deno run --allow-net --allow-read --allow-env vesting_unlock.ts
```