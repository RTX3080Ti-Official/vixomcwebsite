# Play
This server has currently **2** ways of connecting to it.

## Minekube - easiest
Using **Minekube** is the easiest solution, as it just requires connecting to a url. \
To connect with **Minekube** use the URL ``play.vixo.qzz.io`` or ``vixo.play.minekube.net``.

## cloudflared - most stable
Using **cloudflared** helps a lot with stability, as it is a direct connection instead of passing the traffic trought **Minekube**.

### Steps
- Step 1: Install [cloudflared](https://github.com/cloudflare/cloudflared).
- Step 2: In your terminal of choice, run the following command:
```bash
cloudflared access tcp --hostname playtest.vixo.qzz.io --url localhost:5902
```

:::note

You can use whatever port you want, as long as it's not used by another program on your system.

:::

- Step 3: Connect to the server with the address: ``localhost:5902``
- Step 4: Make sure to not close the terminal!

You are now connected to the server via **cloudflared**!