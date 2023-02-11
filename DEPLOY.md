# Deploying parrot on the raspberry pi

- cross-compile for aarch64/armv8/idk:

`cross build --release --target aarch64-unknown-linux-gnu --verbose --features vendored`

- copy to raspberry pi:

`scp target/aarch64-unknown-linux-gnu/release/parrot pi:Programs/parrot/parrot-new`

- then, ssh into pi and stop and remove old parrot etc.
