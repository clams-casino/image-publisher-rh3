# Usage

Turn off duckiebot interface containers first to use camera

Build it on the duckiebot. Assuming in the root directory of the repo
```
dts devel build -f -H <duckiebot name>.local
```

Running it on the duckiebot
```
docker -H <duckiebot name>.local run --rm --privileged --network host <name of the built image>
```

Publishes the images to `/${VEHICLE_NAME}/duckie_cam/compressed`
