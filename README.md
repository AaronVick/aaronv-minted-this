<img src='https://imagedelivery.net/BXluQx4ige9GuW0Ia56BHw/ae8ded7a-9b92-46ca-a19a-03f7014ac600/rectcrop3'/>

# aaronv.eth minted this

a simple script that uses zora api + neynar to check what kind of cool shit @aaronv minted on zora.

I forked the repository built by [@undefined](https://warpcast.com/undefined) for fun because of [this](https://warpcast.com/0xdesigner/0x35c15faa).

[🔗 @0xdesignerminted bot on warpcast](https://warpcast.com/0xdesignerminted)

## stack

simple cron bun script running on a custom server with pm2.

## setup

first copy `.env.example` as `.env` and fill out the necessary info.

```sh
bun install
bun run src/monitor.ts
```

### ❓ why not zora ZDK?

the docs were a little bit outdated and was hard to keep digging types to see what params were correct

### ❓ why not block monitoring using like viem.sh?

developing stuff in web3 for around 9 years, i still think one of the hardest shit to do is block monitoring without failing. it's easy to miss blocks, and things can go haywire when the rpc servers are unstable. going back to dig missed blocks is also painful.

### ❓ why no database?

it's just for 0xdesigner's custom niche case which I then forked. if you wanna build on top of this go ahead.

### ❓ the code looks too hacky?

it's good code if it runs and does its job.
