# alpine-pgbouncer
Minimalistic pgBouncer container with a small disk footprint.

To configure pgBouncer mount an external volume to `/etc/pgbouncer` with the
`pgbouncer.ini` and `userlist.txt` file in them.

## Example Usage

````
docker run --name pgbouncer -d -p 6432:6432 -v /home/core/pgbouncer:/etc/pgbouncer yukimochi/alpine-pgbouncer
````