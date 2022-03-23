[Updater ] __main__                       : Checking for updates...
[Updater ] __main__                       : You're all up to date, enjoy the light show!
Loading configuration file from C:\Users\vku42\AppData\Roaming\.ledfx
Loading default presets from C:\Program Files (x86)\LedFx\data\ledfx
Started webinterface at http://0.0.0.0:8888
Traceback (most recent call last):
  File "C:\Program Files (x86)\LedFx\data\ledfx\effects\audio.py", line 196, in _audio_sample_callback
    self._invoke_callbacks()
  File "C:\Program Files (x86)\LedFx\data\ledfx\effects\audio.py", line 203, in _invoke_callbacks
    callback()
  File "C:\Program Files (x86)\LedFx\data\ledfx\effects\audio.py", line 773, in _audio_data_updated
    self.audio_data_updated(self.audio)
  File "C:\Program Files (x86)\LedFx\data\ledfx\effects\bands(Reactive).py", line 57, in audio_data_updated
    vol = int(out_split[i].max() * band_width)  # length (vol) of band
  File "numpy\core\_methods.py", line 39, in _amax
ValueError: zero-size array to reduction operation maximum which has no identity
[ERROR   ] ledfx.core                     : Exception in core event loop: Task exception was never retrieved
Traceback (most recent call last):
  File "urllib3\util\connection.py", line 86, in create_connection
socket.timeout: timed out

During handling of the above exception, another exception occurred:

Traceback (most recent call last):
  File "core.py", line 117, in async_start
    self.devices.create_from_config(self.config["devices"])
  File "devices\__init__.py", line 313, in create_from_config
  File "devices\__init__.py", line 103, in set_effect
  File "C:\Program Files (x86)\LedFx\data\ledfx\devices\e131.py", line 99, in activate
    if wled_identifier(self.device_ip, self.name):
  File "utils.py", line 129, in wled_identifier
    device_info = requests.get(
  File "requests\api.py", line 76, in get
  File "requests\api.py", line 61, in request
  File "requests\sessions.py", line 542, in request
  File "requests\sessions.py", line 655, in send
  File "requests\adapters.py", line 439, in send
  File "urllib3\connectionpool.py", line 699, in urlopen
  File "urllib3\connectionpool.py", line 394, in _make_request
  File "urllib3\connection.py", line 234, in request
  File "http\client.py", line 1253, in request
  File "http\client.py", line 1299, in _send_request
  File "http\client.py", line 1248, in endheaders
  File "http\client.py", line 1008, in _send_output
  File "http\client.py", line 948, in send
  File "urllib3\connection.py", line 200, in connect
  File "urllib3\connection.py", line 169, in _new_conn
  File "urllib3\util\connection.py", line 86, in create_connection
ValueError
