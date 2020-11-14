# Barrier for Haiku

![Barrier for Haiku](BarrierHaiku.png "Barrier for Haiku")

Barrier for Haiku is a [Barrier](https://github.com/debauchee/barrier) client for the [Haiku Operating System](http://haiku-os.org).

Barrier allows a central machine running the Barrier server to share its Keyboard and Mouse across multiple systems running the client as if they were one desktop.

## Limitations
  - Barrier for Haiku is only a Barrier client at this time
  - Some minor bugs still exist in the keymap translation
  - For now, client name is always "haiku"
  - SSL / TLS is not currently supported and must be disabled on the server

## Compiling
Simply run ```make``` under Haiku

## Configuration
  Create a configuration file at ```~/config/settings/barrier```
  
  ```ini
  enable = true
  server = 192.168.1.101
  server_keymap = "X11"
  ```
### Options
  * **enable**: Enable the client (true|false)
  * **server**: Server address
  * **server_keymap**: Keymap of the Barrier Server (X11|AT)
  * **client_name**: Name of client (string, "haiku" default)
  
## Manual Installation
Copy the barrier_client input add-on to the non-packaged add-ons directory ```~/config/non-packaged/add-ons/input_server/devices/```

## License

Barrier for Haiku is released under the same license as uBarrier (MIT)

## Thanks

Thanks to all of those individuals who have made major contributions to Barrier for Haiku.

* Axel Dörfler (ATKeymap)
* Stefano Ceccherini (wrapper)
* Jérôme Duval (Keymap)
* Alex Evans (uBarrier)
* Jessica Hamilton (wrapper)
* Ed Robbins (wrapper)
