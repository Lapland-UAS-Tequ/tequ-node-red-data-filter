tequ-node-red-data-filter
=====================

Filters data based on value change limit of target value. Timeout can be configured to set regular value updates.

## Install

Run the following command in your Node-RED user directory - typically `~/.node-red`

        npm install tequ-node-red-data-filter

## Information

Filters data based on value change limit of target value. Timeout can be configured to set regular value updates.

Expects following fields set in 'msg' or in node config.
Parameters set in input msg will override node config values.
- msg.target (string, 'msg.payload.d.temperature.v')
- msg.value_change_limit (number, 0-1000000, 0=every value change)
- msg.timeout (number, seconds 0-120)
- msg.deviceId (string)
- msg.deviceType (string)
- msg.topic (string)
