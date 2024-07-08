# PostgreSQL TLS Tester

Simple test of getting a Golang program to connect using TLS to a PostgreSQL bouncer/DB. I needed to build this to troubleshoot why a Golang program was not connecting to a PostgreSQL bouncer. We are using a setup with a CA chain that needed to be sent along with the client's leaf certificate so this program is set up to do that.

## Building

```bash
go build -o pg_tls_tester
```

## Running

```bash
./pg_tls_tester -S service-name
```

or just add any of the other flags to customize it that you can see with `./pg_tls_tester -h`
