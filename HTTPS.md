# Rest API

## `GET /`

Returns the full feature list in JSON(LD) format

## `POST /`

Body contains a feature to update in JSON(LD) format

Returns `{success:true}` if the update succeded or `{success:false,
reason:"reason the update failed"}` otherwise.

## `WEBSOCKET /`

Body contains a feature to watch in JSON(LD) format

Returns feature values when they update

Allowed to fall back to AJAX polling
