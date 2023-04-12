# Comparing `tmp/gradio_client-0.0.9.tar.gz` & `tmp/gradio_client-0.1.0.tar.gz`

## Comparing `gradio_client-0.0.9.tar` & `gradio_client-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0     7462 2020-02-02 00:00:00.000000 gradio_client-0.0.9/README.md
--rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 gradio_client-0.0.9/requirements.txt
--rwxr-xr-x   0        0        0      139 2020-02-02 00:00:00.000000 gradio_client-0.0.9/gradio_client/__init__.py
--rwxr-xr-x   0        0        0    39444 2020-02-02 00:00:00.000000 gradio_client-0.0.9/gradio_client/client.py
--rwxr-xr-x   0        0        0      443 2020-02-02 00:00:00.000000 gradio_client-0.0.9/gradio_client/data_classes.py
--rwxr-xr-x   0        0        0    10765 2020-02-02 00:00:00.000000 gradio_client-0.0.9/gradio_client/documentation.py
--rwxr-xr-x   0        0        0    14859 2020-02-02 00:00:00.000000 gradio_client-0.0.9/gradio_client/serializing.py
--rwxr-xr-x   0        0        0    12276 2020-02-02 00:00:00.000000 gradio_client-0.0.9/gradio_client/utils.py
--rwxr-xr-x   0        0        0        7 2020-02-02 00:00:00.000000 gradio_client-0.0.9/gradio_client/version.txt
--rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 gradio_client-0.0.9/.gitignore
--rwxr-xr-x   0        0        0     1418 2020-02-02 00:00:00.000000 gradio_client-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 gradio_client-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.1.0/README.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.1.0/requirements.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.1.0/gradio_client/__init__.py
+-rw-r--r--   0        0        0    44631 2020-02-02 00:00:00.000000 gradio_client-0.1.0/gradio_client/client.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.1.0/gradio_client/data_classes.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 gradio_client-0.1.0/gradio_client/documentation.py
+-rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 gradio_client-0.1.0/gradio_client/serializing.py
+-rw-r--r--   0        0        0    12618 2020-02-02 00:00:00.000000 gradio_client-0.1.0/gradio_client/utils.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.1.0/gradio_client/version.txt
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gradio_client-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 gradio_client-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 gradio_client-0.1.0/PKG-INFO
```

### Comparing `gradio_client-0.0.9/README.md` & `gradio_client-0.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,212 +1,148 @@
-# `gradio_client`: Use a Gradio app as an API -- in 3 lines of Python
-
-This directory contains the source code for `gradio_client`, a lightweight Python library that makes it very easy to use any Gradio app as an API. 
-
-As an example, consider this [Hugging Face Space that transcribes audio files](https://huggingface.co/spaces/abidlabs/whisper) that are recorded from the microphone.
-
-![](https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/gradio-guides/whisper-screenshot.jpg)
-
-Using the `gradio_client` library, we can easily use the Gradio as an API to transcribe audio files programmatically.
-
-Here's the entire code to do it:
-
-```python
-from gradio_client import Client
-
-client = Client("abidlabs/whisper") 
-client.predict("audio_sample.wav")  
-
->> "This is a test of the whisper speech recognition model."
-```
-
-The Gradio client works with any Gradio Space, whether it be an image generator, a stateful chatbot, or a tax calculator.
-
-## Installation
-
-If you already have a recent version of `gradio`, then the `gradio_client` is included as a dependency. 
-
-Otherwise, the lightweight `gradio_client` package can be installed from pip (or pip3) and works with Python versions 3.9 or higher:
-
-```bash
-$ pip install gradio_client
-```
-
-## Usage
-
-### Connecting to a Space or a Gradio app
-
-Start by connecting instantiating a `Client` object and connecting it to a Gradio app that is running on Spaces (or anywhere else)!
-
-**Connecting to a Space**
-
-```python
-from gradio_client import Client
-
-client = Client("abidlabs/en2fr")  # a Space that translates from English to French
-```
-
-You can also connect to private Spaces by passing in your HF token with the `hf_token` parameter. You can get your HF token here: https://huggingface.co/settings/tokens
-
-```python
-from gradio_client import Client
-
-client = Client("abidlabs/my-private-space", hf_token="...") 
-```
-
-
-**Connecting a general Gradio app**
-
-If your app is running somewhere else, just provide the full URL instead, including the "http://" or "https://". Here's an example of making predictions to a Gradio app that is running on a share URL:
-
-```python
-from gradio_client import Client
-
-client = Client("https://bec81a83-5b5c-471e.gradio.live")
-```
-
-### Inspecting the API endpoints
-
-Once you have connected to a Gradio app, you can view the APIs that are available to you by calling the `Client.view_api()` method. For the Whisper Space, we see the following:
-
-```
-Client.predict() Usage Info
----------------------------
-Named API endpoints: 1
-
- - predict(input_audio, api_name="/predict") -> value_0
-    Parameters:
-     - [Audio] input_audio: str (filepath or URL)
-    Returns:
-     - [Textbox] value_0: str (value)
-```
-
-This shows us that we have 1 API endpoint in this space, and shows us how to use the API endpoint to make a prediction: we should call the `.predict()` method, providing a parameter `input_audio` of type `str`, which is a `filepath or URL`. 
-
-We should also provide the `api_name='/predict'` argument. Although this isn't necessary if a Gradio app has a single named endpoint, it does allow us to call different endpoints in a single app if they are available. If an app has unnamed API endpoints, these can also be displayed by running `.view_api(all_endpoints=True)`.
-
-
-### Making a prediction
-
-The simplest way to make a prediction is simply to call the `.predict()` function with the appropriate arguments:
-
-```python
-from gradio_client import Client
-
-client = Client("abidlabs/en2fr")
-client.predict("Hello")
-
->> Bonjour
-```
-
-If there are multiple parameters, then you should pass them as separate arguments to `.predict()`, like this:
-
-
-```python
-from gradio_client import Client
-
-client = Client("gradio/calculator")
-client.predict(4, "add", 5)
-
->> 9.0
-```
-
-For certain inputs, such as images, you should pass in the filepath or URL to the file. Likewise, for the corresponding output types, you will get a filepath or URL returned. 
-
-```python
-from gradio_client import Client
-
-client = Client("abidlabs/whisper")
-client.predict("https://audio-samples.github.io/samples/mp3/blizzard_unconditional/sample-0.mp3")
-
->> "My thought I have nobody by a beauty and will as you poured. Mr. Rochester is serve in that so don't find simpus, and devoted abode, to at might in a r—"
-```
-
-
-**Running jobs asyncronously**
-
-Oe should note that `.predict()` is a *blocking* operation as it waits for the operation to complete before returning the prediction. 
-
-In many cases, you may be better off letting the job run in the background until you need the results of the prediction. You can do this by creating a `Job` instance using the `.submit()` method, and then later calling `.result()` on the job to get the result. For example:
-
-```python
-from gradio_client import Client
-
-client = Client(space="abidlabs/en2fr")
-job = client.submit("Hello", api_name="/predict")  # This is not blocking
-
-# Do something else
-
-job.result()  # This is blocking
-
->> Bonjour
-```
-
-**Adding callbacks**
-
-Alternatively, one can add one or more callbacks to perform actions after the job has completed running, like this:
-
-```python
-from gradio_client import Client
-
-def print_result(x):
-    print("The translated result is: {x}")
-
-client = Client(space="abidlabs/en2fr")
-
-job = client.submit("Hello", api_name="/predict", result_callbacks=[print_result])
-
-# Do something else
-
->> The translated result is: Bonjour
-
-```
-
-**Status**
-
-The `Job` object also allows you to get the status of the running job by calling the `.status()` method. This returns a `StatusUpdate` object with the following attributes: `code` (the status code, one of a set of defined strings representing the status. See the `utils.Status` class), `rank` (the current position of this job in the queue), `queue_size` (the total queue size),  `eta` (estimated time this job will complete), `success` (a boolean representing whether the job completed successfully), and `time` (the time that the status was generated). 
-
-```py
-from gradio_client import Client
-
-client = Client(src="gradio/calculator")
-job = client.submit(5, "add", 4, api_name="/predict")
-job.status()
-
->> <Status.STARTING: 'STARTING'>
-```
-
-The `Job` object also has a `done()` instance method which returns a boolean indicating whether the job has completed.
-
-### Generator Endpoints
-
-Some Gradio API endpoints do not return a single value, rather they return a series of values. You can get the series of values that have been returned at any time from such a generator endpoint by running `job.outputs()`:
-
-```py
-from gradio_client import Client
-
-client = Client(src="gradio/count_generator")
-job = client.submit(3, api_name="/count")
-while not job.done():
-    time.sleep(0.1)
-job.outputs()
-
->> ['0', '1', '2']
-```
-
-Note that running `job.result()` on a generator endpoint only gives you the *first* value returned by the endpoint. 
-
-The `Job` object is also iterable, which means you can use it to display the results of a generator function as they are returned from the endpoint. Here's the equivalent example using the `Job` as a generator:
-
-```py
-from gradio_client import Client
-
-client = Client(src="gradio/count_generator")
-job = client.submit(3, api_name="/count")
-
-for o in job:
-    print(o)
-
->> 0
->> 1
->> 2
-```
+# `gradio_client`: Use a Gradio app as an API -- in 3 lines of Python
+
+This directory contains the source code for `gradio_client`, a lightweight Python library that makes it very easy to use any Gradio app as an API. 
+
+As an example, consider this [Hugging Face Space that transcribes audio files](https://huggingface.co/spaces/abidlabs/whisper) that are recorded from the microphone.
+
+![](https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/gradio-guides/whisper-screenshot.jpg)
+
+Using the `gradio_client` library, we can easily use the Gradio as an API to transcribe audio files programmatically.
+
+Here's the entire code to do it:
+
+```python
+from gradio_client import Client
+
+client = Client("abidlabs/whisper") 
+client.predict("audio_sample.wav")  
+
+>> "This is a test of the whisper speech recognition model."
+```
+
+The Gradio client works with any Gradio Space, whether it be an image generator, a stateful chatbot, or a tax calculator.
+
+## Installation
+
+If you already have a recent version of `gradio`, then the `gradio_client` is included as a dependency. 
+
+Otherwise, the lightweight `gradio_client` package can be installed from pip (or pip3) and works with Python versions 3.9 or higher:
+
+```bash
+$ pip install gradio_client
+```
+
+## Basic Usage
+
+### Connecting to a Space or a Gradio app
+
+Start by connecting instantiating a `Client` object and connecting it to a Gradio app that is running on Spaces (or anywhere else)!
+
+**Connecting to a Space**
+
+```python
+from gradio_client import Client
+
+client = Client("abidlabs/en2fr")  # a Space that translates from English to French
+```
+
+You can also connect to private Spaces by passing in your HF token with the `hf_token` parameter. You can get your HF token here: https://huggingface.co/settings/tokens
+
+```python
+from gradio_client import Client
+
+client = Client("abidlabs/my-private-space", hf_token="...") 
+```
+
+**Duplicating a Space for private use**
+
+While you can use any public Space as an API, you may get rate limited by Hugging Face if you make too many requests. For unlimited usage of a Space, simply duplicate the Space to create a private Space,
+and then use it to make as many requests as you'd like!
+
+The `gradio_client` includes a class method: `Client.duplicate()` to make this process simple:
+
+```python
+from gradio_client import Client
+
+client = Client.duplicate("abidlabs/whisper") 
+client.predict("audio_sample.wav")  
+
+>> "This is a test of the whisper speech recognition model."
+```
+
+If you have previously duplicated a Space, re-running `duplicate()` will *not* create a new Space. Instead, the Client will attach to the previously-created Space. So it is safe to re-run the `Client.duplicate()` method multiple times. 
+
+**Note:** if the original Space uses GPUs, your private Space will as well, and your Hugging Face account will get billed based on the price of the GPU. To minimize charges, your Space will automatically go to sleep after 1 hour of inactivity. You can also set the hardware using the `hardware` parameter of `duplicate()`.
+
+
+**Connecting a general Gradio app**
+
+If your app is running somewhere else, just provide the full URL instead, including the "http://" or "https://". Here's an example of making predictions to a Gradio app that is running on a share URL:
+
+```python
+from gradio_client import Client
+
+client = Client("https://bec81a83-5b5c-471e.gradio.live")
+```
+
+
+### Inspecting the API endpoints
+
+Once you have connected to a Gradio app, you can view the APIs that are available to you by calling the `.view_api()` method. For the Whisper Space, we see the following:
+
+```
+Client.predict() Usage Info
+---------------------------
+Named API endpoints: 1
+
+ - predict(input_audio, api_name="/predict") -> value_0
+    Parameters:
+     - [Audio] input_audio: str (filepath or URL)
+    Returns:
+     - [Textbox] value_0: str (value)
+```
+
+This shows us that we have 1 API endpoint in this space, and shows us how to use the API endpoint to make a prediction: we should call the `.predict()` method, providing a parameter `input_audio` of type `str`, which is a `filepath or URL`. 
+
+We should also provide the `api_name='/predict'` argument. Although this isn't necessary if a Gradio app has a single named endpoint, it does allow us to call different endpoints in a single app if they are available. If an app has unnamed API endpoints, these can also be displayed by running `.view_api(all_endpoints=True)`.
+
+
+### Making a prediction
+
+The simplest way to make a prediction is simply to call the `.predict()` function with the appropriate arguments:
+
+```python
+from gradio_client import Client
+
+client = Client("abidlabs/en2fr")
+client.predict("Hello")
+
+>> Bonjour
+```
+
+If there are multiple parameters, then you should pass them as separate arguments to `.predict()`, like this:
+
+
+```python
+from gradio_client import Client
+
+client = Client("gradio/calculator")
+client.predict(4, "add", 5)
+
+>> 9.0
+```
+
+For certain inputs, such as images, you should pass in the filepath or URL to the file. Likewise, for the corresponding output types, you will get a filepath or URL returned. 
+
+```python
+from gradio_client import Client
+
+client = Client("abidlabs/whisper")
+client.predict("https://audio-samples.github.io/samples/mp3/blizzard_unconditional/sample-0.mp3")
+
+>> "My thought I have nobody by a beauty and will as you poured. Mr. Rochester is serve in that so don't find simpus, and devoted abode, to at might in a r—"
+```
+
+
+## Advanced Usage
+
+For more ways to use the Gradio Python Client, check out our dedicated Guide on the Python client, available here: https://www.gradio.app/getting-started-with-the-python-client/
```

### Comparing `gradio_client-0.0.9/gradio_client/client.py` & `gradio_client-0.1.0/gradio_client/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,912 +1,1030 @@
-"""The main Client class for the Python client."""
-from __future__ import annotations
-
-import concurrent.futures
-import json
-import re
-import threading
-import time
-import urllib.parse
-import uuid
-from concurrent.futures import Future, TimeoutError
-from datetime import datetime
-from pathlib import Path
-from threading import Lock
-from typing import Any, Callable, Dict, List, Tuple
-
-import huggingface_hub
-import requests
-import websockets
-from huggingface_hub.utils import build_hf_headers, send_telemetry
-from packaging import version
-from typing_extensions import Literal
-
-from gradio_client import serializing, utils
-from gradio_client.documentation import document, set_documentation_group
-from gradio_client.serializing import Serializable
-from gradio_client.utils import Communicator, JobStatus, Status, StatusUpdate
-
-set_documentation_group("py-client")
-
-
-@document("predict", "submit", "view_api")
-class Client:
-    """
-    The main Client class for the Python client. This class is used to connect to a remote Gradio app and call its API endpoints.
-
-    Example:
-        from gradio_client import Client
-
-        client = Client("abidlabs/whisper-large-v2")  # connecting to a Hugging Face Space
-        client.predict("test.mp4", api_name="/predict")
-        >> What a nice recording! # returns the result of the remote API call
-
-        client = Client("https://bec81a83-5b5c-471e.gradio.live")  # connecting to a temporary Gradio share URL
-        job = client.submit("hello", api_name="/predict")  # runs the prediction in a background thread
-        job.result()
-        >> 49 # returns the result of the remote API call (blocking call)
-
-    """
-
-    def __init__(
-        self,
-        src: str,
-        hf_token: str | None = None,
-        max_workers: int = 40,
-        verbose: bool = True,
-    ):
-        """
-        Parameters:
-            src: Either the name of the Hugging Face Space to load, (e.g. "abidlabs/whisper-large-v2") or the full URL (including "http" or "https") of the hosted Gradio app to load (e.g. "http://mydomain.com/app" or "https://bec81a83-5b5c-471e.gradio.live/").
-            hf_token: The Hugging Face token to use to access private Spaces. Automatically fetched if you are logged in via the Hugging Face Hub CLI.
-            max_workers: The maximum number of thread workers that can be used to make requests to the remote Gradio app simultaneously.
-            verbose: Whether the client should print statements to the console.
-        """
-        self.verbose = verbose
-        self.hf_token = hf_token
-        self.headers = build_hf_headers(
-            token=hf_token,
-            library_name="gradio_client",
-            library_version=utils.__version__,
-        )
-        self.space_id = None
-
-        if src.startswith("http://") or src.startswith("https://"):
-            _src = src
-        else:
-            _src = self._space_name_to_src(src)
-            if _src is None:
-                raise ValueError(
-                    f"Could not find Space: {src}. If it is a private Space, please provide an hf_token."
-                )
-            self.space_id = src
-        self.src = _src
-        if self.verbose:
-            print(f"Loaded as API: {self.src} ✔")
-
-        print("self.src", self.src)
-        self.api_url = urllib.parse.urljoin(self.src, utils.API_URL)
-        self.ws_url = urllib.parse.urljoin(
-            self.src.replace("http", "ws", 1), utils.WS_URL
-        )
-        self.upload_url = urllib.parse.urljoin(self.src, utils.UPLOAD_URL)
-        self.reset_url = urllib.parse.urljoin(self.src, utils.RESET_URL)
-        self.config = self._get_config()
-        self.session_hash = str(uuid.uuid4())
-
-        self.endpoints = [
-            Endpoint(self, fn_index, dependency)
-            for fn_index, dependency in enumerate(self.config["dependencies"])
-        ]
-
-        # Create a pool of threads to handle the requests
-        self.executor = concurrent.futures.ThreadPoolExecutor(max_workers=max_workers)
-
-        # Disable telemetry by setting the env variable HF_HUB_DISABLE_TELEMETRY=1
-        threading.Thread(target=self._telemetry_thread).start()
-
-    def predict(
-        self,
-        *args,
-        api_name: str | None = None,
-        fn_index: int | None = None,
-    ) -> Any:
-        """
-        Calls the Gradio API and returns the result (this is a blocking call).
-
-        Parameters:
-            args: The arguments to pass to the remote API. The order of the arguments must match the order of the inputs in the Gradio app.
-            api_name: The name of the API endpoint to call starting with a leading slash, e.g. "/predict". Does not need to be provided if the Gradio app has only one named API endpoint.
-            fn_index: As an alternative to api_name, this parameter takes the index of the API endpoint to call, e.g. 0. Both api_name and fn_index can be provided, but if they conflict, api_name will take precedence.
-        Returns:
-            The result of the API call. Will be a Tuple if the API has multiple outputs.
-        Example:
-            from gradio_client import Client
-            client = Client(src="gradio/calculator")
-            client.predict(5, "add", 4, api_name="/predict")
-            >> 9.0
-        """
-        return self.submit(*args, api_name=api_name, fn_index=fn_index).result()
-
-    def submit(
-        self,
-        *args,
-        api_name: str | None = None,
-        fn_index: int | None = None,
-        result_callbacks: Callable | List[Callable] | None = None,
-    ) -> Job:
-        """
-        Creates and returns a Job object which calls the Gradio API in a background thread. The job can be used to retrieve the status and result of the remote API call.
-
-        Parameters:
-            args: The arguments to pass to the remote API. The order of the arguments must match the order of the inputs in the Gradio app.
-            api_name: The name of the API endpoint to call starting with a leading slash, e.g. "/predict". Does not need to be provided if the Gradio app has only one named API endpoint.
-            fn_index: As an alternative to api_name, this parameter takes the index of the API endpoint to call, e.g. 0. Both api_name and fn_index can be provided, but if they conflict, api_name will take precedence.
-            result_callbacks: A callback function, or list of callback functions, to be called when the result is ready. If a list of functions is provided, they will be called in order. The return values from the remote API are provided as separate parameters into the callback. If None, no callback will be called.
-        Returns:
-            A Job object that can be used to retrieve the status and result of the remote API call.
-        Example:
-            from gradio_client import Client
-            client = Client(src="gradio/calculator")
-            job = client.submit(5, "add", 4, api_name="/predict")
-            job.status()
-            >> <Status.STARTING: 'STARTING'>
-            job.result()  # blocking call
-            >> 9.0
-        """
-        inferred_fn_index = self._infer_fn_index(api_name, fn_index)
-
-        helper = None
-        if self.endpoints[inferred_fn_index].use_ws:
-            helper = Communicator(
-                Lock(),
-                JobStatus(),
-                self.endpoints[inferred_fn_index].deserialize,
-                self.reset_url,
-            )
-        end_to_end_fn = self.endpoints[inferred_fn_index].make_end_to_end_fn(helper)
-        future = self.executor.submit(end_to_end_fn, *args)
-
-        job = Job(
-            future, communicator=helper, verbose=self.verbose, space_id=self.space_id
-        )
-
-        if result_callbacks:
-            if isinstance(result_callbacks, Callable):
-                result_callbacks = [result_callbacks]
-
-            def create_fn(callback) -> Callable:
-                def fn(future):
-                    if isinstance(future.result(), tuple):
-                        callback(*future.result())
-                    else:
-                        callback(future.result())
-
-                return fn
-
-            for callback in result_callbacks:
-                job.add_done_callback(create_fn(callback))
-
-        return job
-
-    def view_api(
-        self,
-        all_endpoints: bool | None = None,
-        print_info: bool = True,
-        return_format: Literal["dict", "str"] | None = None,
-    ) -> Dict | str | None:
-        """
-        Prints the usage info for the API. If the Gradio app has multiple API endpoints, the usage info for each endpoint will be printed separately. If return_format="dict" the info is returned in dictionary format, as shown in the example below.
-
-        Parameters:
-            all_endpoints: If True, prints information for both named and unnamed endpoints in the Gradio app. If False, will only print info about named endpoints. If None (default), will only print info about unnamed endpoints if there are no named endpoints.
-            print_info: If True, prints the usage info to the console. If False, does not print the usage info.
-            return_format: If None, nothing is returned. If "str", returns the same string that would be printed to the console. If "dict", returns the usage info as a dictionary that can be programmatically parsed, and *all endpoints are returned in the dictionary* regardless of the value of `all_endpoints`. The format of the dictionary is in the docstring of this method.
-        Example:
-            from gradio_client import Client
-            client = Client(src="gradio/calculator")
-            client.view_api(return_format="dict")
-            >> {
-                'named_endpoints': {
-                    '/predict': {
-                        'parameters': {
-                            'num1': ['int | float', 'value', 'Number'],
-                            'operation': ['str', 'value', 'Radio'],
-                            'num2': ['int | float', 'value', 'Number']
-                            },
-                        'returns': {
-                            'output': ['int | float', 'value', 'Number']
-                            }
-                        }
-                    },
-                'unnamed_endpoints': {
-                    2: {
-                        'parameters': {
-                            'parameter_0': ['str', 'value', 'Dataset']
-                            },
-                        'returns': {
-                            'num1': ['int | float', 'value', 'Number'],
-                            'operation': ['str', 'value', 'Radio'],
-                            'num2': ['int | float', 'value', 'Number'],
-                            'output': ['int | float', 'value', 'Number']
-                            }
-                        }
-                    }
-                }
-            }
-
-        """
-        info: Dict[str, Dict[str | int, Dict[str, Dict[str, List[str]]]]] = {
-            "named_endpoints": {},
-            "unnamed_endpoints": {},
-        }
-
-        for endpoint in self.endpoints:
-            if endpoint.is_valid:
-                if endpoint.api_name:
-                    info["named_endpoints"][endpoint.api_name] = endpoint.get_info()
-                else:
-                    info["unnamed_endpoints"][endpoint.fn_index] = endpoint.get_info()
-
-        num_named_endpoints = len(info["named_endpoints"])
-        num_unnamed_endpoints = len(info["unnamed_endpoints"])
-        if num_named_endpoints == 0 and all_endpoints is None:
-            all_endpoints = True
-
-        human_info = "Client.predict() Usage Info\n---------------------------\n"
-        human_info += f"Named API endpoints: {num_named_endpoints}\n"
-
-        for api_name, endpoint_info in info["named_endpoints"].items():
-            human_info += self._render_endpoints_info(api_name, endpoint_info)
-
-        if all_endpoints:
-            human_info += f"\nUnnamed API endpoints: {num_unnamed_endpoints}\n"
-            for fn_index, endpoint_info in info["unnamed_endpoints"].items():
-                human_info += self._render_endpoints_info(fn_index, endpoint_info)
-        else:
-            if num_unnamed_endpoints > 0:
-                human_info += f"\nUnnamed API endpoints: {num_unnamed_endpoints}, to view, run Client.view_api(`all_endpoints=True`)\n"
-
-        if print_info:
-            print(human_info)
-        if return_format == "str":
-            return human_info
-        elif return_format == "dict":
-            return info
-
-    def reset_session(self) -> None:
-        self.session_hash = str(uuid.uuid4())
-
-    def _render_endpoints_info(
-        self,
-        name_or_index: str | int,
-        endpoints_info: Dict[str, Dict[str, List[str]]],
-    ) -> str:
-        parameter_names = list(endpoints_info["parameters"].keys())
-        rendered_parameters = ", ".join(parameter_names)
-        if rendered_parameters:
-            rendered_parameters = rendered_parameters + ", "
-        return_value_names = list(endpoints_info["returns"].keys())
-        rendered_return_values = ", ".join(return_value_names)
-        if len(return_value_names) > 1:
-            rendered_return_values = f"({rendered_return_values})"
-
-        if isinstance(name_or_index, str):
-            final_param = f'api_name="{name_or_index}"'
-        elif isinstance(name_or_index, int):
-            final_param = f"fn_index={name_or_index}"
-        else:
-            raise ValueError("name_or_index must be a string or integer")
-
-        human_info = f"\n - predict({rendered_parameters}{final_param}) -> {rendered_return_values}\n"
-        human_info += "    Parameters:\n"
-        if endpoints_info["parameters"]:
-            for label, info in endpoints_info["parameters"].items():
-                human_info += f"     - [{info[2]}] {label}: {info[0]} ({info[1]})\n"
-        else:
-            human_info += "     - None\n"
-        human_info += "    Returns:\n"
-        if endpoints_info["returns"]:
-            for label, info in endpoints_info["returns"].items():
-                human_info += f"     - [{info[2]}] {label}: {info[0]} ({info[1]})\n"
-        else:
-            human_info += "     - None\n"
-
-        return human_info
-
-    def __repr__(self):
-        return self.view_api(print_info=False, return_format="str")
-
-    def __str__(self):
-        return self.view_api(print_info=False, return_format="str")
-
-    def _telemetry_thread(self) -> None:
-        # Disable telemetry by setting the env variable HF_HUB_DISABLE_TELEMETRY=1
-        data = {
-            "src": self.src,
-        }
-        try:
-            send_telemetry(
-                topic="py_client/initiated",
-                library_name="gradio_client",
-                library_version=utils.__version__,
-                user_agent=data,
-            )
-        except Exception:
-            pass
-
-    def _infer_fn_index(self, api_name: str | None, fn_index: int | None) -> int:
-        inferred_fn_index = None
-        if api_name is not None:
-            for i, d in enumerate(self.config["dependencies"]):
-                config_api_name = d.get("api_name")
-                if config_api_name is None:
-                    continue
-                if "/" + config_api_name == api_name:
-                    inferred_fn_index = i
-                    break
-            else:
-                error_message = f"Cannot find a function with `api_name`: {api_name}."
-                if not api_name.startswith("/"):
-                    error_message += " Did you mean to use a leading slash?"
-                raise ValueError(error_message)
-        elif fn_index is not None:
-            inferred_fn_index = fn_index
-        else:
-            valid_endpoints = [
-                e for e in self.endpoints if e.is_valid and e.api_name is not None
-            ]
-            if len(valid_endpoints) == 1:
-                inferred_fn_index = valid_endpoints[0].fn_index
-            else:
-                raise ValueError(
-                    "This Gradio app might have multiple endpoints. Please specify an `api_name` or `fn_index`"
-                )
-        return inferred_fn_index
-
-    def __del__(self):
-        if hasattr(self, "executor"):
-            self.executor.shutdown(wait=True)
-
-    def _space_name_to_src(self, space) -> str | None:
-        return huggingface_hub.space_info(space, token=self.hf_token).host  # type: ignore
-
-    def _get_config(self) -> Dict:
-        assert self.src is not None
-        r = requests.get(self.src, headers=self.headers)
-        # some basic regex to extract the config
-        result = re.search(r"window.gradio_config = (.*?);[\s]*</script>", r.text)
-        try:
-            config = json.loads(result.group(1))  # type: ignore
-        except AttributeError:
-            raise ValueError(f"Could not get Gradio config from: {self.src}")
-        if "allow_flagging" in config:
-            raise ValueError(
-                "Gradio 2.x is not supported by this client. Please upgrade your Gradio app to Gradio 3.x or higher."
-            )
-        return config
-
-
-class Endpoint:
-    """Helper class for storing all the information about a single API endpoint."""
-
-    def __init__(self, client: Client, fn_index: int, dependency: Dict):
-        self.client: Client = client
-        self.fn_index = fn_index
-        self.dependency = dependency
-        self.api_name: str | None = dependency.get("api_name")
-        if self.api_name:
-            self.api_name = "/" + self.api_name
-        self.use_ws = self._use_websocket(self.dependency)
-        self.input_component_types = []
-        self.output_component_types = []
-        self.root_url = client.src + "/" if not client.src.endswith("/") else client.src
-        try:
-            self.serializers, self.deserializers = self._setup_serializers()
-            self.is_valid = self.dependency[
-                "backend_fn"
-            ]  # Only a real API endpoint if backend_fn is True and serializers are valid
-        except AssertionError:
-            self.is_valid = False
-
-    def get_info(self) -> Dict[str, Dict[str, List[str]]]:
-        """
-        Dictionary format:
-            {
-                "parameters": {
-                    "parameter_1_name": ["type", "description", "component_type"],
-                    "parameter_2_name": ["type", "description", "component_type"],
-                    ...
-                },
-                "returns": {
-                    "value_1_name": ["type", "description", "component_type"],
-                    ...
-                }
-            }
-        """
-        parameters = {}
-        for i, input in enumerate(self.dependency["inputs"]):
-            for component in self.client.config["components"]:
-                if component["id"] == input:
-                    label = (
-                        component["props"]
-                        .get("label", f"parameter_{i}")
-                        .lower()
-                        .replace(" ", "_")
-                    )
-                    if "info" in component:
-                        info = component["info"]["input"]
-                    else:
-                        info = self.serializers[i].input_api_info()
-                    info = list(info)
-                    component_type = component.get("type", "component").capitalize()
-                    info.append(component_type)
-                    if not component_type.lower() == utils.STATE_COMPONENT:
-                        parameters[label] = info
-        returns = {}
-        for o, output in enumerate(self.dependency["outputs"]):
-            for component in self.client.config["components"]:
-                if component["id"] == output:
-                    label = (
-                        component["props"]
-                        .get("label", f"value_{o}")
-                        .lower()
-                        .replace(" ", "_")
-                    )
-                    if "info" in component:
-                        info = component["info"]["output"]
-                    else:
-                        info = self.deserializers[o].output_api_info()
-                    info = list(info)
-                    component_type = component.get("type", "component").capitalize()
-                    info.append(component_type)
-                    if not component_type.lower() == utils.STATE_COMPONENT:
-                        returns[label] = info
-
-        return {"parameters": parameters, "returns": returns}
-
-    def __repr__(self):
-        return json.dumps(self.get_info(), indent=4)
-
-    def __str__(self):
-        return json.dumps(self.get_info(), indent=4)
-
-    def make_end_to_end_fn(self, helper: Communicator | None = None):
-
-        _predict = self.make_predict(helper)
-
-        def _inner(*data):
-            if not self.is_valid:
-                raise utils.InvalidAPIEndpointError()
-            inputs = self.serialize(*data)
-            predictions = _predict(*inputs)
-            output = self.deserialize(*predictions)
-            # Append final output only if not already present
-            # for consistency between generators and not generators
-            if helper:
-                with helper.lock:
-                    if not helper.job.outputs:
-                        helper.job.outputs.append(output)
-            return output
-
-        return _inner
-
-    def make_predict(self, helper: Communicator | None = None):
-        def _predict(*data) -> Tuple:
-            data = json.dumps(
-                {
-                    "data": data,
-                    "fn_index": self.fn_index,
-                    "session_hash": self.client.session_hash,
-                }
-            )
-            hash_data = json.dumps(
-                {
-                    "fn_index": self.fn_index,
-                    "session_hash": self.client.session_hash,
-                }
-            )
-
-            if self.use_ws:
-                result = utils.synchronize_async(self._ws_fn, data, hash_data, helper)
-                output = result["data"]
-            else:
-                response = requests.post(
-                    self.client.api_url, headers=self.client.headers, data=data
-                )
-                result = json.loads(response.content.decode("utf-8"))
-                try:
-                    output = result["data"]
-                except KeyError:
-                    if "error" in result and "429" in result["error"]:
-                        raise utils.TooManyRequestsError(
-                            "Too many requests to the Hugging Face API"
-                        )
-                    raise KeyError(
-                        f"Could not find 'data' key in response. Response received: {result}"
-                    )
-            return tuple(output)
-
-        return _predict
-
-    def _predict_resolve(self, *data) -> Any:
-        """Needed for gradio.load(), which has a slightly different signature for serializing/deserializing"""
-        outputs = self.make_predict()(*data)
-        if len(self.dependency["outputs"]) == 1:
-            return outputs[0]
-        return outputs
-
-    def _upload(
-        self, file_paths: List[str | List[str]]
-    ) -> List[str | List[str]] | List[Dict[str, Any] | List[Dict[str, Any]]]:
-        if not file_paths:
-            return []
-        # Put all the filepaths in one file
-        # but then keep track of which index in the
-        # original list they came from so we can recreate
-        # the original structure
-        files = []
-        indices = []
-        for i, fs in enumerate(file_paths):
-            if not isinstance(fs, list):
-                fs = [fs]
-            for f in fs:
-                files.append(("files", (Path(f).name, open(f, "rb"))))
-                indices.append(i)
-        r = requests.post(
-            self.client.upload_url, headers=self.client.headers, files=files
-        )
-        if r.status_code != 200:
-            uploaded = file_paths
-        else:
-            uploaded = []
-            result = r.json()
-            for i, fs in enumerate(file_paths):
-                if isinstance(fs, list):
-                    output = [o for ix, o in enumerate(result) if indices[ix] == i]
-                    res = [
-                        {
-                            "is_file": True,
-                            "name": o,
-                            "orig_name": Path(f).name,
-                            "data": None,
-                        }
-                        for f, o in zip(fs, output)
-                    ]
-                else:
-                    o = next(o for ix, o in enumerate(result) if indices[ix] == i)
-                    res = {
-                        "is_file": True,
-                        "name": o,
-                        "orig_name": Path(fs).name,
-                        "data": None,
-                    }
-                uploaded.append(res)
-        return uploaded
-
-    def _add_uploaded_files_to_data(
-        self,
-        files: List[str | List[str]] | List[Dict[str, Any] | List[Dict[str, Any]]],
-        data: List[Any],
-    ) -> None:
-        """Helper function to modify the input data with the uploaded files."""
-        file_counter = 0
-        for i, t in enumerate(self.input_component_types):
-            if t in ["file", "uploadbutton"]:
-                data[i] = files[file_counter]
-                file_counter += 1
-
-    def serialize(self, *data) -> Tuple:
-        data = list(data)
-        for i, input_component_type in enumerate(self.input_component_types):
-            if input_component_type == utils.STATE_COMPONENT:
-                data.insert(i, None)
-        assert len(data) == len(
-            self.serializers
-        ), f"Expected {len(self.serializers)} arguments, got {len(data)}"
-
-        files = [
-            f
-            for f, t in zip(data, self.input_component_types)
-            if t in ["file", "uploadbutton"]
-        ]
-        uploaded_files = self._upload(files)
-        self._add_uploaded_files_to_data(uploaded_files, data)
-
-        o = tuple([s.serialize(d) for s, d in zip(self.serializers, data)])
-        return o
-
-    def deserialize(self, *data) -> Tuple | Any:
-        assert len(data) == len(
-            self.deserializers
-        ), f"Expected {len(self.deserializers)} outputs, got {len(data)}"
-        outputs = tuple(
-            [
-                s.deserialize(d, hf_token=self.client.hf_token, root_url=self.root_url)
-                for s, d, oct in zip(
-                    self.deserializers, data, self.output_component_types
-                )
-                if not oct == utils.STATE_COMPONENT
-            ]
-        )
-        if (
-            len(
-                [
-                    oct
-                    for oct in self.output_component_types
-                    if not oct == utils.STATE_COMPONENT
-                ]
-            )
-            == 1
-        ):
-            output = outputs[0]
-        else:
-            output = outputs
-        return output
-
-    def _setup_serializers(self) -> Tuple[List[Serializable], List[Serializable]]:
-        inputs = self.dependency["inputs"]
-        serializers = []
-
-        for i in inputs:
-            for component in self.client.config["components"]:
-                if component["id"] == i:
-                    component_name = component["type"]
-                    self.input_component_types.append(component_name)
-                    if component.get("serializer"):
-                        serializer_name = component["serializer"]
-                        assert (
-                            serializer_name in serializing.SERIALIZER_MAPPING
-                        ), f"Unknown serializer: {serializer_name}, you may need to update your gradio_client version."
-                        serializer = serializing.SERIALIZER_MAPPING[serializer_name]
-                    else:
-                        assert (
-                            component_name in serializing.COMPONENT_MAPPING
-                        ), f"Unknown component: {component_name}, you may need to update your gradio_client version."
-                        serializer = serializing.COMPONENT_MAPPING[component_name]
-                    serializers.append(serializer())  # type: ignore
-
-        outputs = self.dependency["outputs"]
-        deserializers = []
-        for i in outputs:
-            for component in self.client.config["components"]:
-                if component["id"] == i:
-                    component_name = component["type"]
-                    self.output_component_types.append(component_name)
-                    if component.get("serializer"):
-                        serializer_name = component["serializer"]
-                        assert (
-                            serializer_name in serializing.SERIALIZER_MAPPING
-                        ), f"Unknown serializer: {serializer_name}, you may need to update your gradio_client version."
-                        deserializer = serializing.SERIALIZER_MAPPING[serializer_name]
-                    else:
-                        assert (
-                            component_name in serializing.COMPONENT_MAPPING
-                        ), f"Unknown component: {component_name}, you may need to update your gradio_client version."
-                        deserializer = serializing.COMPONENT_MAPPING[component_name]
-                    deserializers.append(deserializer())  # type: ignore
-
-        return serializers, deserializers
-
-    def _use_websocket(self, dependency: Dict) -> bool:
-        queue_enabled = self.client.config.get("enable_queue", False)
-        queue_uses_websocket = version.parse(
-            self.client.config.get("version", "2.0")
-        ) >= version.Version("3.2")
-        dependency_uses_queue = dependency.get("queue", False) is not False
-        return queue_enabled and queue_uses_websocket and dependency_uses_queue
-
-    async def _ws_fn(self, data, hash_data, helper: Communicator):
-        async with websockets.connect(  # type: ignore
-            self.client.ws_url,
-            open_timeout=10,
-            extra_headers=self.client.headers,
-            max_size=1024 * 1024 * 1024,
-        ) as websocket:
-            return await utils.get_pred_from_ws(websocket, data, hash_data, helper)
-
-
-@document("result", "outputs", "status")
-class Job(Future):
-    """
-    A Job is a wrapper over the Future class that represents a prediction call that has been
-    submitted by the Gradio client. This class is not meant to be instantiated directly, but rather
-    is created by the Client.submit() method.
-
-    A Job object includes methods to get the status of the prediction call, as well to get the outputs of
-    the prediction call. Job objects are also iterable, and can be used in a loop to get the outputs
-    of prediction calls as they become available for generator endpoints.
-    """
-
-    def __init__(
-        self,
-        future: Future,
-        communicator: Communicator | None = None,
-        verbose: bool = True,
-        space_id: str | None = None,
-    ):
-        """
-        Parameters:
-            future: The future object that represents the prediction call, created by the Client.submit() method
-            communicator: The communicator object that is used to communicate between the client and the background thread running the job
-            verbose: Whether to print any status-related messages to the console
-            space_id: The space ID corresponding to the Client object that created this Job object
-        """
-        self.future = future
-        self.communicator = communicator
-        self._counter = 0
-        self.verbose = verbose
-        self.space_id = space_id
-
-    def __iter__(self) -> Job:
-        return self
-
-    def __next__(self) -> Tuple | Any:
-        if not self.communicator:
-            raise StopIteration()
-
-        with self.communicator.lock:
-            if self.communicator.job.latest_status.code == Status.FINISHED:
-                raise StopIteration()
-
-        while True:
-            with self.communicator.lock:
-                if len(self.communicator.job.outputs) == self._counter + 1:
-                    o = self.communicator.job.outputs[self._counter]
-                    self._counter += 1
-                    return o
-                if self.communicator.job.latest_status.code == Status.FINISHED:
-                    raise StopIteration()
-
-    def result(self, timeout=None) -> Any:
-        """
-        Return the result of the call that the future represents. Raises CancelledError: If the future was cancelled, TimeoutError: If the future didn't finish executing before the given timeout, and Exception: If the call raised then that exception will be raised.
-
-        Parameters:
-            timeout: The number of seconds to wait for the result if the future isn't done. If None, then there is no limit on the wait time.
-        Returns:
-            The result of the call that the future represents.
-        Example:
-            from gradio_client import Client
-            calculator = Client(src="gradio/calculator")
-            job = calculator.submit("foo", "add", 4, fn_index=0)
-            job.result(timeout=5)
-            >> 9
-        """
-        if self.communicator:
-            timeout = timeout or float("inf")
-            if self.future._exception:  # type: ignore
-                raise self.future._exception  # type: ignore
-            with self.communicator.lock:
-                if self.communicator.job.outputs:
-                    return self.communicator.job.outputs[0]
-            start = datetime.now()
-            while True:
-                if (datetime.now() - start).seconds > timeout:
-                    raise TimeoutError()
-                if self.future._exception:  # type: ignore
-                    raise self.future._exception  # type: ignore
-                with self.communicator.lock:
-                    if self.communicator.job.outputs:
-                        return self.communicator.job.outputs[0]
-                time.sleep(0.01)
-        else:
-            return super().result(timeout=timeout)
-
-    def outputs(self) -> List[Tuple | Any]:
-        """
-        Returns a list containing the latest outputs from the Job.
-
-        If the endpoint has multiple output components, the list will contain
-        a tuple of results. Otherwise, it will contain the results without storing them
-        in tuples.
-
-        For endpoints that are queued, this list will contain the final job output even
-        if that endpoint does not use a generator function.
-
-        Example:
-            from gradio_client import Client
-            client = Client(src="gradio/count_generator")
-            job = client.submit(3, api_name="/count")
-            while not job.done():
-                time.sleep(0.1)
-            job.outputs()
-            >> ['0', '1', '2']
-        """
-        if not self.communicator:
-            return []
-        else:
-            with self.communicator.lock:
-                return self.communicator.job.outputs
-
-    def status(self) -> StatusUpdate:
-        """
-        Returns the latest status update from the Job in the form of a StatusUpdate
-        object, which contains the following fields: code, rank, queue_size, success, time, eta.
-
-        Example:
-            from gradio_client import Client
-            client = Client(src="gradio/calculator")
-            job = client.submit(5, "add", 4, api_name="/predict")
-            job.status()
-            >> <Status.STARTING: 'STARTING'>
-            job.status().eta
-            >> 43.241  # seconds
-        """
-        time = datetime.now()
-        cancelled = False
-        if self.communicator:
-            with self.communicator.lock:
-                cancelled = self.communicator.should_cancel
-        if cancelled:
-            return StatusUpdate(
-                code=Status.CANCELLED,
-                rank=0,
-                queue_size=None,
-                success=False,
-                time=time,
-                eta=None,
-            )
-        if self.done():
-            if not self.future._exception:  # type: ignore
-                return StatusUpdate(
-                    code=Status.FINISHED,
-                    rank=0,
-                    queue_size=None,
-                    success=True,
-                    time=time,
-                    eta=None,
-                )
-            else:
-                return StatusUpdate(
-                    code=Status.FINISHED,
-                    rank=0,
-                    queue_size=None,
-                    success=False,
-                    time=time,
-                    eta=None,
-                )
-        else:
-            if not self.communicator:
-                return StatusUpdate(
-                    code=Status.PROCESSING,
-                    rank=0,
-                    queue_size=None,
-                    success=None,
-                    time=time,
-                    eta=None,
-                )
-            else:
-                with self.communicator.lock:
-                    eta = self.communicator.job.latest_status.eta
-                    if self.verbose and self.space_id and eta and eta > 30:
-                        print(
-                            f"Due to heavy traffic on this app, the prediction will take approximately {int(eta)} seconds."
-                            f"For faster predictions without waiting in queue, you may duplicate the space: {utils.DUPLICATE_URL.format(self.space_id)}"
-                        )
-                    return self.communicator.job.latest_status
-
-    def __getattr__(self, name):
-        """Forwards any properties to the Future class."""
-        return getattr(self.future, name)
-
-    def cancel(self) -> bool:
-        """Cancels the job as best as possible.
-
-        If the app you are connecting to has the gradio queue enabled, the job
-        will be cancelled locally as soon as possible. For apps that do not use the
-        queue, the job cannot be cancelled if it's been sent to the local executor
-        (for the time being).
-
-        Note: In general, this DOES not stop the process from running in the upstream server
-        except for the following situations:
-
-        1. If the job is queued upstream, it will be removed from the queue and the server will not run the job
-        2. If the job has iterative outputs, the job will finish as soon as the current iteration finishes running
-        3. If the job has not been picked up by the queue yet, the queue will not pick up the job
-        """
-        if self.communicator:
-            with self.communicator.lock:
-                self.communicator.should_cancel = True
-                return True
-        return self.future.cancel()
+"""The main Client class for the Python client."""
+from __future__ import annotations
+
+import concurrent.futures
+import json
+import re
+import threading
+import time
+import urllib.parse
+import uuid
+from concurrent.futures import Future, TimeoutError
+from datetime import datetime
+from pathlib import Path
+from threading import Lock
+from typing import Any, Callable, Dict, List, Tuple
+
+import huggingface_hub
+import requests
+import websockets
+from huggingface_hub.utils import (
+    RepositoryNotFoundError,
+    build_hf_headers,
+    send_telemetry,
+)
+from packaging import version
+from typing_extensions import Literal
+
+from gradio_client import serializing, utils
+from gradio_client.documentation import document, set_documentation_group
+from gradio_client.serializing import Serializable
+from gradio_client.utils import Communicator, JobStatus, Status, StatusUpdate
+
+set_documentation_group("py-client")
+
+
+@document("predict", "submit", "view_api")
+class Client:
+    """
+    The main Client class for the Python client. This class is used to connect to a remote Gradio app and call its API endpoints.
+
+    Example:
+        from gradio_client import Client
+
+        client = Client("abidlabs/whisper-large-v2")  # connecting to a Hugging Face Space
+        client.predict("test.mp4", api_name="/predict")
+        >> What a nice recording! # returns the result of the remote API call
+
+        client = Client("https://bec81a83-5b5c-471e.gradio.live")  # connecting to a temporary Gradio share URL
+        job = client.submit("hello", api_name="/predict")  # runs the prediction in a background thread
+        job.result()
+        >> 49 # returns the result of the remote API call (blocking call)
+
+    """
+
+    def __init__(
+        self,
+        src: str,
+        hf_token: str | None = None,
+        max_workers: int = 40,
+        verbose: bool = True,
+    ):
+        """
+        Parameters:
+            src: Either the name of the Hugging Face Space to load, (e.g. "abidlabs/whisper-large-v2") or the full URL (including "http" or "https") of the hosted Gradio app to load (e.g. "http://mydomain.com/app" or "https://bec81a83-5b5c-471e.gradio.live/").
+            hf_token: The Hugging Face token to use to access private Spaces. Automatically fetched if you are logged in via the Hugging Face Hub CLI. Obtain from: https://huggingface.co/settings/token
+            max_workers: The maximum number of thread workers that can be used to make requests to the remote Gradio app simultaneously.
+            verbose: Whether the client should print statements to the console.
+        """
+        self.verbose = verbose
+        self.hf_token = hf_token
+        self.headers = build_hf_headers(
+            token=hf_token,
+            library_name="gradio_client",
+            library_version=utils.__version__,
+        )
+        self.space_id = None
+
+        if src.startswith("http://") or src.startswith("https://"):
+            _src = src
+        else:
+            _src = self._space_name_to_src(src)
+            if _src is None:
+                raise ValueError(
+                    f"Could not find Space: {src}. If it is a private Space, please provide an hf_token."
+                )
+            self.space_id = src
+        self.src = _src
+        state = self._get_space_state()
+        if state == utils.BUILDING_RUNTIME:
+            if self.verbose:
+                print("Space is still building. Please wait...")
+            while self._get_space_state() == utils.BUILDING_RUNTIME:
+                time.sleep(2)  # so we don't get rate limited by the API
+                pass
+        if state in utils.INVALID_RUNTIME:
+            raise ValueError(
+                f"The current space is in the invalid state: {state}. "
+                "Please contact the owner to fix this."
+            )
+        if self.verbose:
+            print(f"Loaded as API: {self.src} ✔")
+
+        self.api_url = urllib.parse.urljoin(self.src, utils.API_URL)
+        self.ws_url = urllib.parse.urljoin(
+            self.src.replace("http", "ws", 1), utils.WS_URL
+        )
+        self.upload_url = urllib.parse.urljoin(self.src, utils.UPLOAD_URL)
+        self.reset_url = urllib.parse.urljoin(self.src, utils.RESET_URL)
+        self.config = self._get_config()
+        self.session_hash = str(uuid.uuid4())
+
+        self.endpoints = [
+            Endpoint(self, fn_index, dependency)
+            for fn_index, dependency in enumerate(self.config["dependencies"])
+        ]
+
+        # Create a pool of threads to handle the requests
+        self.executor = concurrent.futures.ThreadPoolExecutor(max_workers=max_workers)
+
+        # Disable telemetry by setting the env variable HF_HUB_DISABLE_TELEMETRY=1
+        threading.Thread(target=self._telemetry_thread).start()
+
+    @classmethod
+    def duplicate(
+        cls,
+        from_id: str,
+        to_id: str | None = None,
+        hf_token: str | None = None,
+        private: bool = True,
+        hardware: str | None = None,
+        secrets: Dict[str, str] | None = None,
+        sleep_timeout: int = 5,
+        max_workers: int = 40,
+        verbose: bool = True,
+    ):
+        """
+        Duplicates a Hugging Face Space under your account and returns a Client object
+        for the new Space. No duplication is created if the Space already exists in your
+        account (to override this, provide a new name for the new Space using `to_id`).
+        To use this method, you must provide an `hf_token` or be logged in via the Hugging
+        Face Hub CLI.
+
+        The new Space will be private by default and use the same hardware as the original
+        Space. This can be changed by using the `private` and `hardware` parameters. For
+        hardware upgrades (beyond the basic CPU tier), you may be required to provide
+        billing information on Hugging Face: https://huggingface.co/settings/billing
+
+        Parameters:
+            from_id: The name of the Hugging Face Space to duplicate in the format "{username}/{space_id}", e.g. "gradio/whisper".
+            to_id: The name of the new Hugging Face Space to create, e.g. "abidlabs/whisper-duplicate". If not provided, the new Space will be named "{your_HF_username}/{space_id}".
+            hf_token: The Hugging Face token to use to access private Spaces. Automatically fetched if you are logged in via the Hugging Face Hub CLI. Obtain from: https://huggingface.co/settings/token
+            private: Whether the new Space should be private (True) or public (False). Defaults to True.
+            hardware: The hardware tier to use for the new Space. Defaults to the same hardware tier as the original Space. Options include "cpu-basic", "cpu-upgrade", "t4-small", "t4-medium", "a10g-small", "a10g-large", "a100-large", subject to availability.
+            secrets: A dictionary of (secret key, secret value) to pass to the new Space. Defaults to None.
+            sleep_timeout: The number of minutes after which the duplicate Space will be puased if no requests are made to it (to minimize billing charges). Defaults to 5 minutes.
+            max_workers: The maximum number of thread workers that can be used to make requests to the remote Gradio app simultaneously.
+            verbose: Whether the client should print statements to the console.
+        """
+        try:
+            info = huggingface_hub.get_space_runtime(from_id, token=hf_token)
+        except RepositoryNotFoundError:
+            raise ValueError(
+                f"Could not find Space: {from_id}. If it is a private Space, please provide an `hf_token`."
+            )
+        if to_id:
+            if "/" in to_id:
+                to_id = to_id.split("/")[1]
+            space_id = huggingface_hub.get_full_repo_name(to_id, token=hf_token)
+        else:
+            space_id = huggingface_hub.get_full_repo_name(
+                from_id.split("/")[1], token=hf_token
+            )
+        try:
+            huggingface_hub.get_space_runtime(space_id, token=hf_token)
+            if verbose:
+                print(
+                    f"Using your existing Space: {utils.SPACE_URL.format(space_id)} 🤗"
+                )
+        except RepositoryNotFoundError:
+            if verbose:
+                print(f"Creating a duplicate of {from_id} for your own use... 🤗")
+            huggingface_hub.duplicate_space(
+                from_id=from_id,
+                to_id=space_id,
+                token=hf_token,
+                exist_ok=True,
+                private=private,
+            )
+            utils.set_space_timeout(
+                space_id, hf_token=hf_token, timeout_in_seconds=sleep_timeout * 60
+            )
+            if verbose:
+                print(f"Created new Space: {utils.SPACE_URL.format(space_id)}")
+        current_info = huggingface_hub.get_space_runtime(space_id, token=hf_token)
+        current_hardware = current_info.hardware or "cpu-basic"
+        if hardware is None:
+            hardware = info.hardware
+        if not current_hardware == hardware:
+            huggingface_hub.request_space_hardware(space_id, hardware)  # type: ignore
+            print(
+                f"-------\nNOTE: this Space uses upgraded hardware: {hardware}... see billing info at https://huggingface.co/settings/billing\n-------"
+            )
+        if secrets is not None:
+            for key, value in secrets.items():
+                huggingface_hub.add_space_secret(space_id, key, value, token=hf_token)
+        if verbose:
+            print("")
+        client = cls(
+            space_id, hf_token=hf_token, max_workers=max_workers, verbose=verbose
+        )
+        return client
+
+    def _get_space_state(self):
+        if not self.space_id:
+            return None
+        info = huggingface_hub.get_space_runtime(self.space_id, token=self.hf_token)
+        return info.stage
+
+    def predict(
+        self,
+        *args,
+        api_name: str | None = None,
+        fn_index: int | None = None,
+    ) -> Any:
+        """
+        Calls the Gradio API and returns the result (this is a blocking call).
+
+        Parameters:
+            args: The arguments to pass to the remote API. The order of the arguments must match the order of the inputs in the Gradio app.
+            api_name: The name of the API endpoint to call starting with a leading slash, e.g. "/predict". Does not need to be provided if the Gradio app has only one named API endpoint.
+            fn_index: As an alternative to api_name, this parameter takes the index of the API endpoint to call, e.g. 0. Both api_name and fn_index can be provided, but if they conflict, api_name will take precedence.
+        Returns:
+            The result of the API call. Will be a Tuple if the API has multiple outputs.
+        Example:
+            from gradio_client import Client
+            client = Client(src="gradio/calculator")
+            client.predict(5, "add", 4, api_name="/predict")
+            >> 9.0
+        """
+        return self.submit(*args, api_name=api_name, fn_index=fn_index).result()
+
+    def submit(
+        self,
+        *args,
+        api_name: str | None = None,
+        fn_index: int | None = None,
+        result_callbacks: Callable | List[Callable] | None = None,
+    ) -> Job:
+        """
+        Creates and returns a Job object which calls the Gradio API in a background thread. The job can be used to retrieve the status and result of the remote API call.
+
+        Parameters:
+            args: The arguments to pass to the remote API. The order of the arguments must match the order of the inputs in the Gradio app.
+            api_name: The name of the API endpoint to call starting with a leading slash, e.g. "/predict". Does not need to be provided if the Gradio app has only one named API endpoint.
+            fn_index: As an alternative to api_name, this parameter takes the index of the API endpoint to call, e.g. 0. Both api_name and fn_index can be provided, but if they conflict, api_name will take precedence.
+            result_callbacks: A callback function, or list of callback functions, to be called when the result is ready. If a list of functions is provided, they will be called in order. The return values from the remote API are provided as separate parameters into the callback. If None, no callback will be called.
+        Returns:
+            A Job object that can be used to retrieve the status and result of the remote API call.
+        Example:
+            from gradio_client import Client
+            client = Client(src="gradio/calculator")
+            job = client.submit(5, "add", 4, api_name="/predict")
+            job.status()
+            >> <Status.STARTING: 'STARTING'>
+            job.result()  # blocking call
+            >> 9.0
+        """
+        inferred_fn_index = self._infer_fn_index(api_name, fn_index)
+
+        helper = None
+        if self.endpoints[inferred_fn_index].use_ws:
+            helper = Communicator(
+                Lock(),
+                JobStatus(),
+                self.endpoints[inferred_fn_index].deserialize,
+                self.reset_url,
+            )
+        end_to_end_fn = self.endpoints[inferred_fn_index].make_end_to_end_fn(helper)
+        future = self.executor.submit(end_to_end_fn, *args)
+
+        job = Job(
+            future, communicator=helper, verbose=self.verbose, space_id=self.space_id
+        )
+
+        if result_callbacks:
+            if isinstance(result_callbacks, Callable):
+                result_callbacks = [result_callbacks]
+
+            def create_fn(callback) -> Callable:
+                def fn(future):
+                    if isinstance(future.result(), tuple):
+                        callback(*future.result())
+                    else:
+                        callback(future.result())
+
+                return fn
+
+            for callback in result_callbacks:
+                job.add_done_callback(create_fn(callback))
+
+        return job
+
+    def view_api(
+        self,
+        all_endpoints: bool | None = None,
+        print_info: bool = True,
+        return_format: Literal["dict", "str"] | None = None,
+    ) -> Dict | str | None:
+        """
+        Prints the usage info for the API. If the Gradio app has multiple API endpoints, the usage info for each endpoint will be printed separately. If return_format="dict" the info is returned in dictionary format, as shown in the example below.
+
+        Parameters:
+            all_endpoints: If True, prints information for both named and unnamed endpoints in the Gradio app. If False, will only print info about named endpoints. If None (default), will only print info about unnamed endpoints if there are no named endpoints.
+            print_info: If True, prints the usage info to the console. If False, does not print the usage info.
+            return_format: If None, nothing is returned. If "str", returns the same string that would be printed to the console. If "dict", returns the usage info as a dictionary that can be programmatically parsed, and *all endpoints are returned in the dictionary* regardless of the value of `all_endpoints`. The format of the dictionary is in the docstring of this method.
+        Example:
+            from gradio_client import Client
+            client = Client(src="gradio/calculator")
+            client.view_api(return_format="dict")
+            >> {
+                'named_endpoints': {
+                    '/predict': {
+                        'parameters': {
+                            'num1': ['int | float', 'value', 'Number'],
+                            'operation': ['str', 'value', 'Radio'],
+                            'num2': ['int | float', 'value', 'Number']
+                            },
+                        'returns': {
+                            'output': ['int | float', 'value', 'Number']
+                            }
+                        }
+                    },
+                'unnamed_endpoints': {
+                    2: {
+                        'parameters': {
+                            'parameter_0': ['str', 'value', 'Dataset']
+                            },
+                        'returns': {
+                            'num1': ['int | float', 'value', 'Number'],
+                            'operation': ['str', 'value', 'Radio'],
+                            'num2': ['int | float', 'value', 'Number'],
+                            'output': ['int | float', 'value', 'Number']
+                            }
+                        }
+                    }
+                }
+            }
+
+        """
+        info: Dict[str, Dict[str | int, Dict[str, Dict[str, List[str]]]]] = {
+            "named_endpoints": {},
+            "unnamed_endpoints": {},
+        }
+
+        for endpoint in self.endpoints:
+            if endpoint.is_valid:
+                if endpoint.api_name:
+                    info["named_endpoints"][endpoint.api_name] = endpoint.get_info()
+                else:
+                    info["unnamed_endpoints"][endpoint.fn_index] = endpoint.get_info()
+
+        num_named_endpoints = len(info["named_endpoints"])
+        num_unnamed_endpoints = len(info["unnamed_endpoints"])
+        if num_named_endpoints == 0 and all_endpoints is None:
+            all_endpoints = True
+
+        human_info = "Client.predict() Usage Info\n---------------------------\n"
+        human_info += f"Named API endpoints: {num_named_endpoints}\n"
+
+        for api_name, endpoint_info in info["named_endpoints"].items():
+            human_info += self._render_endpoints_info(api_name, endpoint_info)
+
+        if all_endpoints:
+            human_info += f"\nUnnamed API endpoints: {num_unnamed_endpoints}\n"
+            for fn_index, endpoint_info in info["unnamed_endpoints"].items():
+                human_info += self._render_endpoints_info(fn_index, endpoint_info)
+        else:
+            if num_unnamed_endpoints > 0:
+                human_info += f"\nUnnamed API endpoints: {num_unnamed_endpoints}, to view, run Client.view_api(`all_endpoints=True`)\n"
+
+        if print_info:
+            print(human_info)
+        if return_format == "str":
+            return human_info
+        elif return_format == "dict":
+            return info
+
+    def reset_session(self) -> None:
+        self.session_hash = str(uuid.uuid4())
+
+    def _render_endpoints_info(
+        self,
+        name_or_index: str | int,
+        endpoints_info: Dict[str, Dict[str, List[str]]],
+    ) -> str:
+        parameter_names = list(endpoints_info["parameters"].keys())
+        rendered_parameters = ", ".join(parameter_names)
+        if rendered_parameters:
+            rendered_parameters = rendered_parameters + ", "
+        return_value_names = list(endpoints_info["returns"].keys())
+        rendered_return_values = ", ".join(return_value_names)
+        if len(return_value_names) > 1:
+            rendered_return_values = f"({rendered_return_values})"
+
+        if isinstance(name_or_index, str):
+            final_param = f'api_name="{name_or_index}"'
+        elif isinstance(name_or_index, int):
+            final_param = f"fn_index={name_or_index}"
+        else:
+            raise ValueError("name_or_index must be a string or integer")
+
+        human_info = f"\n - predict({rendered_parameters}{final_param}) -> {rendered_return_values}\n"
+        human_info += "    Parameters:\n"
+        if endpoints_info["parameters"]:
+            for label, info in endpoints_info["parameters"].items():
+                human_info += f"     - [{info[2]}] {label}: {info[0]} ({info[1]})\n"
+        else:
+            human_info += "     - None\n"
+        human_info += "    Returns:\n"
+        if endpoints_info["returns"]:
+            for label, info in endpoints_info["returns"].items():
+                human_info += f"     - [{info[2]}] {label}: {info[0]} ({info[1]})\n"
+        else:
+            human_info += "     - None\n"
+
+        return human_info
+
+    def __repr__(self):
+        return self.view_api(print_info=False, return_format="str")
+
+    def __str__(self):
+        return self.view_api(print_info=False, return_format="str")
+
+    def _telemetry_thread(self) -> None:
+        # Disable telemetry by setting the env variable HF_HUB_DISABLE_TELEMETRY=1
+        data = {
+            "src": self.src,
+        }
+        try:
+            send_telemetry(
+                topic="py_client/initiated",
+                library_name="gradio_client",
+                library_version=utils.__version__,
+                user_agent=data,
+            )
+        except Exception:
+            pass
+
+    def _infer_fn_index(self, api_name: str | None, fn_index: int | None) -> int:
+        inferred_fn_index = None
+        if api_name is not None:
+            for i, d in enumerate(self.config["dependencies"]):
+                config_api_name = d.get("api_name")
+                if config_api_name is None:
+                    continue
+                if "/" + config_api_name == api_name:
+                    inferred_fn_index = i
+                    break
+            else:
+                error_message = f"Cannot find a function with `api_name`: {api_name}."
+                if not api_name.startswith("/"):
+                    error_message += " Did you mean to use a leading slash?"
+                raise ValueError(error_message)
+        elif fn_index is not None:
+            inferred_fn_index = fn_index
+        else:
+            valid_endpoints = [
+                e for e in self.endpoints if e.is_valid and e.api_name is not None
+            ]
+            if len(valid_endpoints) == 1:
+                inferred_fn_index = valid_endpoints[0].fn_index
+            else:
+                raise ValueError(
+                    "This Gradio app might have multiple endpoints. Please specify an `api_name` or `fn_index`"
+                )
+        return inferred_fn_index
+
+    def __del__(self):
+        if hasattr(self, "executor"):
+            self.executor.shutdown(wait=True)
+
+    def _space_name_to_src(self, space) -> str | None:
+        return huggingface_hub.space_info(space, token=self.hf_token).host  # type: ignore
+
+    def _get_config(self) -> Dict:
+        assert self.src is not None
+        r = requests.get(self.src, headers=self.headers)
+        # some basic regex to extract the config
+        result = re.search(r"window.gradio_config = (.*?);[\s]*</script>", r.text)
+        try:
+            config = json.loads(result.group(1))  # type: ignore
+        except AttributeError:
+            raise ValueError(f"Could not get Gradio config from: {self.src}")
+        if "allow_flagging" in config:
+            raise ValueError(
+                "Gradio 2.x is not supported by this client. Please upgrade your Gradio app to Gradio 3.x or higher."
+            )
+        return config
+
+
+class Endpoint:
+    """Helper class for storing all the information about a single API endpoint."""
+
+    def __init__(self, client: Client, fn_index: int, dependency: Dict):
+        self.client: Client = client
+        self.fn_index = fn_index
+        self.dependency = dependency
+        self.api_name: str | None = dependency.get("api_name")
+        if self.api_name:
+            self.api_name = "/" + self.api_name
+        self.use_ws = self._use_websocket(self.dependency)
+        self.input_component_types = []
+        self.output_component_types = []
+        self.root_url = client.src + "/" if not client.src.endswith("/") else client.src
+        try:
+            self.serializers, self.deserializers = self._setup_serializers()
+            self.is_valid = self.dependency[
+                "backend_fn"
+            ]  # Only a real API endpoint if backend_fn is True and serializers are valid
+        except AssertionError:
+            self.is_valid = False
+
+    def get_info(self) -> Dict[str, Dict[str, List[str]]]:
+        """
+        Dictionary format:
+            {
+                "parameters": {
+                    "parameter_1_name": ["type", "description", "component_type"],
+                    "parameter_2_name": ["type", "description", "component_type"],
+                    ...
+                },
+                "returns": {
+                    "value_1_name": ["type", "description", "component_type"],
+                    ...
+                }
+            }
+        """
+        parameters = {}
+        for i, input in enumerate(self.dependency["inputs"]):
+            for component in self.client.config["components"]:
+                if component["id"] == input:
+                    label = (
+                        component["props"]
+                        .get("label", f"parameter_{i}")
+                        .lower()
+                        .replace(" ", "_")
+                    )
+                    if "info" in component:
+                        info = component["info"]["input"]
+                    else:
+                        info = self.serializers[i].input_api_info()
+                    info = list(info)
+                    component_type = component.get("type", "component").capitalize()
+                    info.append(component_type)
+                    if not component_type.lower() == utils.STATE_COMPONENT:
+                        parameters[label] = info
+        returns = {}
+        for o, output in enumerate(self.dependency["outputs"]):
+            for component in self.client.config["components"]:
+                if component["id"] == output:
+                    label = (
+                        component["props"]
+                        .get("label", f"value_{o}")
+                        .lower()
+                        .replace(" ", "_")
+                    )
+                    if "info" in component:
+                        info = component["info"]["output"]
+                    else:
+                        info = self.deserializers[o].output_api_info()
+                    info = list(info)
+                    component_type = component.get("type", "component").capitalize()
+                    info.append(component_type)
+                    if not component_type.lower() == utils.STATE_COMPONENT:
+                        returns[label] = info
+
+        return {"parameters": parameters, "returns": returns}
+
+    def __repr__(self):
+        return json.dumps(self.get_info(), indent=4)
+
+    def __str__(self):
+        return json.dumps(self.get_info(), indent=4)
+
+    def make_end_to_end_fn(self, helper: Communicator | None = None):
+
+        _predict = self.make_predict(helper)
+
+        def _inner(*data):
+            if not self.is_valid:
+                raise utils.InvalidAPIEndpointError()
+            inputs = self.serialize(*data)
+            predictions = _predict(*inputs)
+            output = self.deserialize(*predictions)
+            # Append final output only if not already present
+            # for consistency between generators and not generators
+            if helper:
+                with helper.lock:
+                    if not helper.job.outputs:
+                        helper.job.outputs.append(output)
+            return output
+
+        return _inner
+
+    def make_predict(self, helper: Communicator | None = None):
+        def _predict(*data) -> Tuple:
+            data = json.dumps(
+                {
+                    "data": data,
+                    "fn_index": self.fn_index,
+                    "session_hash": self.client.session_hash,
+                }
+            )
+            hash_data = json.dumps(
+                {
+                    "fn_index": self.fn_index,
+                    "session_hash": self.client.session_hash,
+                }
+            )
+
+            if self.use_ws:
+                result = utils.synchronize_async(self._ws_fn, data, hash_data, helper)
+                if "error" in result:
+                    raise ValueError(result["error"])
+            else:
+                response = requests.post(
+                    self.client.api_url, headers=self.client.headers, data=data
+                )
+                result = json.loads(response.content.decode("utf-8"))
+            try:
+                output = result["data"]
+            except KeyError:
+                is_public_space = (
+                    self.client.space_id
+                    and not huggingface_hub.space_info(self.client.space_id).private
+                )
+                if "error" in result and "429" in result["error"] and is_public_space:
+                    raise utils.TooManyRequestsError(
+                        f"Too many requests to the API, please try again later. To avoid being rate-limited, please duplicate the Space using Client.duplicate({self.client.space_id}) and pass in your Hugging Face token."
+                    )
+                elif "error" in result:
+                    raise ValueError(result["error"])
+                raise KeyError(
+                    f"Could not find 'data' key in response. Response received: {result}"
+                )
+            return tuple(output)
+
+        return _predict
+
+    def _predict_resolve(self, *data) -> Any:
+        """Needed for gradio.load(), which has a slightly different signature for serializing/deserializing"""
+        outputs = self.make_predict()(*data)
+        if len(self.dependency["outputs"]) == 1:
+            return outputs[0]
+        return outputs
+
+    def _upload(
+        self, file_paths: List[str | List[str]]
+    ) -> List[str | List[str]] | List[Dict[str, Any] | List[Dict[str, Any]]]:
+        if not file_paths:
+            return []
+        # Put all the filepaths in one file
+        # but then keep track of which index in the
+        # original list they came from so we can recreate
+        # the original structure
+        files = []
+        indices = []
+        for i, fs in enumerate(file_paths):
+            if not isinstance(fs, list):
+                fs = [fs]
+            for f in fs:
+                files.append(("files", (Path(f).name, open(f, "rb"))))
+                indices.append(i)
+        r = requests.post(
+            self.client.upload_url, headers=self.client.headers, files=files
+        )
+        if r.status_code != 200:
+            uploaded = file_paths
+        else:
+            uploaded = []
+            result = r.json()
+            for i, fs in enumerate(file_paths):
+                if isinstance(fs, list):
+                    output = [o for ix, o in enumerate(result) if indices[ix] == i]
+                    res = [
+                        {
+                            "is_file": True,
+                            "name": o,
+                            "orig_name": Path(f).name,
+                            "data": None,
+                        }
+                        for f, o in zip(fs, output)
+                    ]
+                else:
+                    o = next(o for ix, o in enumerate(result) if indices[ix] == i)
+                    res = {
+                        "is_file": True,
+                        "name": o,
+                        "orig_name": Path(fs).name,
+                        "data": None,
+                    }
+                uploaded.append(res)
+        return uploaded
+
+    def _add_uploaded_files_to_data(
+        self,
+        files: List[str | List[str]] | List[Dict[str, Any] | List[Dict[str, Any]]],
+        data: List[Any],
+    ) -> None:
+        """Helper function to modify the input data with the uploaded files."""
+        file_counter = 0
+        for i, t in enumerate(self.input_component_types):
+            if t in ["file", "uploadbutton"]:
+                data[i] = files[file_counter]
+                file_counter += 1
+
+    def serialize(self, *data) -> Tuple:
+        data = list(data)
+        for i, input_component_type in enumerate(self.input_component_types):
+            if input_component_type == utils.STATE_COMPONENT:
+                data.insert(i, None)
+        assert len(data) == len(
+            self.serializers
+        ), f"Expected {len(self.serializers)} arguments, got {len(data)}"
+
+        files = [
+            f
+            for f, t in zip(data, self.input_component_types)
+            if t in ["file", "uploadbutton"]
+        ]
+        uploaded_files = self._upload(files)
+        self._add_uploaded_files_to_data(uploaded_files, data)
+
+        o = tuple([s.serialize(d) for s, d in zip(self.serializers, data)])
+        return o
+
+    def deserialize(self, *data) -> Tuple | Any:
+        assert len(data) == len(
+            self.deserializers
+        ), f"Expected {len(self.deserializers)} outputs, got {len(data)}"
+        outputs = tuple(
+            [
+                s.deserialize(d, hf_token=self.client.hf_token, root_url=self.root_url)
+                for s, d, oct in zip(
+                    self.deserializers, data, self.output_component_types
+                )
+                if not oct == utils.STATE_COMPONENT
+            ]
+        )
+        if (
+            len(
+                [
+                    oct
+                    for oct in self.output_component_types
+                    if not oct == utils.STATE_COMPONENT
+                ]
+            )
+            == 1
+        ):
+            output = outputs[0]
+        else:
+            output = outputs
+        return output
+
+    def _setup_serializers(self) -> Tuple[List[Serializable], List[Serializable]]:
+        inputs = self.dependency["inputs"]
+        serializers = []
+
+        for i in inputs:
+            for component in self.client.config["components"]:
+                if component["id"] == i:
+                    component_name = component["type"]
+                    self.input_component_types.append(component_name)
+                    if component.get("serializer"):
+                        serializer_name = component["serializer"]
+                        assert (
+                            serializer_name in serializing.SERIALIZER_MAPPING
+                        ), f"Unknown serializer: {serializer_name}, you may need to update your gradio_client version."
+                        serializer = serializing.SERIALIZER_MAPPING[serializer_name]
+                    else:
+                        assert (
+                            component_name in serializing.COMPONENT_MAPPING
+                        ), f"Unknown component: {component_name}, you may need to update your gradio_client version."
+                        serializer = serializing.COMPONENT_MAPPING[component_name]
+                    serializers.append(serializer())  # type: ignore
+
+        outputs = self.dependency["outputs"]
+        deserializers = []
+        for i in outputs:
+            for component in self.client.config["components"]:
+                if component["id"] == i:
+                    component_name = component["type"]
+                    self.output_component_types.append(component_name)
+                    if component.get("serializer"):
+                        serializer_name = component["serializer"]
+                        assert (
+                            serializer_name in serializing.SERIALIZER_MAPPING
+                        ), f"Unknown serializer: {serializer_name}, you may need to update your gradio_client version."
+                        deserializer = serializing.SERIALIZER_MAPPING[serializer_name]
+                    else:
+                        assert (
+                            component_name in serializing.COMPONENT_MAPPING
+                        ), f"Unknown component: {component_name}, you may need to update your gradio_client version."
+                        deserializer = serializing.COMPONENT_MAPPING[component_name]
+                    deserializers.append(deserializer())  # type: ignore
+
+        return serializers, deserializers
+
+    def _use_websocket(self, dependency: Dict) -> bool:
+        queue_enabled = self.client.config.get("enable_queue", False)
+        queue_uses_websocket = version.parse(
+            self.client.config.get("version", "2.0")
+        ) >= version.Version("3.2")
+        dependency_uses_queue = dependency.get("queue", False) is not False
+        return queue_enabled and queue_uses_websocket and dependency_uses_queue
+
+    async def _ws_fn(self, data, hash_data, helper: Communicator):
+        async with websockets.connect(  # type: ignore
+            self.client.ws_url,
+            open_timeout=10,
+            extra_headers=self.client.headers,
+            max_size=1024 * 1024 * 1024,
+        ) as websocket:
+            return await utils.get_pred_from_ws(websocket, data, hash_data, helper)
+
+
+@document("result", "outputs", "status")
+class Job(Future):
+    """
+    A Job is a wrapper over the Future class that represents a prediction call that has been
+    submitted by the Gradio client. This class is not meant to be instantiated directly, but rather
+    is created by the Client.submit() method.
+
+    A Job object includes methods to get the status of the prediction call, as well to get the outputs of
+    the prediction call. Job objects are also iterable, and can be used in a loop to get the outputs
+    of prediction calls as they become available for generator endpoints.
+    """
+
+    def __init__(
+        self,
+        future: Future,
+        communicator: Communicator | None = None,
+        verbose: bool = True,
+        space_id: str | None = None,
+    ):
+        """
+        Parameters:
+            future: The future object that represents the prediction call, created by the Client.submit() method
+            communicator: The communicator object that is used to communicate between the client and the background thread running the job
+            verbose: Whether to print any status-related messages to the console
+            space_id: The space ID corresponding to the Client object that created this Job object
+        """
+        self.future = future
+        self.communicator = communicator
+        self._counter = 0
+        self.verbose = verbose
+        self.space_id = space_id
+
+    def __iter__(self) -> Job:
+        return self
+
+    def __next__(self) -> Tuple | Any:
+        if not self.communicator:
+            raise StopIteration()
+
+        with self.communicator.lock:
+            if self.communicator.job.latest_status.code == Status.FINISHED:
+                raise StopIteration()
+
+        while True:
+            with self.communicator.lock:
+                if len(self.communicator.job.outputs) == self._counter + 1:
+                    o = self.communicator.job.outputs[self._counter]
+                    self._counter += 1
+                    return o
+                if self.communicator.job.latest_status.code == Status.FINISHED:
+                    raise StopIteration()
+
+    def result(self, timeout=None) -> Any:
+        """
+        Return the result of the call that the future represents. Raises CancelledError: If the future was cancelled, TimeoutError: If the future didn't finish executing before the given timeout, and Exception: If the call raised then that exception will be raised.
+
+        Parameters:
+            timeout: The number of seconds to wait for the result if the future isn't done. If None, then there is no limit on the wait time.
+        Returns:
+            The result of the call that the future represents.
+        Example:
+            from gradio_client import Client
+            calculator = Client(src="gradio/calculator")
+            job = calculator.submit("foo", "add", 4, fn_index=0)
+            job.result(timeout=5)
+            >> 9
+        """
+        if self.communicator:
+            timeout = timeout or float("inf")
+            if self.future._exception:  # type: ignore
+                raise self.future._exception  # type: ignore
+            with self.communicator.lock:
+                if self.communicator.job.outputs:
+                    return self.communicator.job.outputs[0]
+            start = datetime.now()
+            while True:
+                if (datetime.now() - start).seconds > timeout:
+                    raise TimeoutError()
+                if self.future._exception:  # type: ignore
+                    raise self.future._exception  # type: ignore
+                with self.communicator.lock:
+                    if self.communicator.job.outputs:
+                        return self.communicator.job.outputs[0]
+                time.sleep(0.01)
+        else:
+            return super().result(timeout=timeout)
+
+    def outputs(self) -> List[Tuple | Any]:
+        """
+        Returns a list containing the latest outputs from the Job.
+
+        If the endpoint has multiple output components, the list will contain
+        a tuple of results. Otherwise, it will contain the results without storing them
+        in tuples.
+
+        For endpoints that are queued, this list will contain the final job output even
+        if that endpoint does not use a generator function.
+
+        Example:
+            from gradio_client import Client
+            client = Client(src="gradio/count_generator")
+            job = client.submit(3, api_name="/count")
+            while not job.done():
+                time.sleep(0.1)
+            job.outputs()
+            >> ['0', '1', '2']
+        """
+        if not self.communicator:
+            return []
+        else:
+            with self.communicator.lock:
+                return self.communicator.job.outputs
+
+    def status(self) -> StatusUpdate:
+        """
+        Returns the latest status update from the Job in the form of a StatusUpdate
+        object, which contains the following fields: code, rank, queue_size, success, time, eta.
+
+        Example:
+            from gradio_client import Client
+            client = Client(src="gradio/calculator")
+            job = client.submit(5, "add", 4, api_name="/predict")
+            job.status()
+            >> <Status.STARTING: 'STARTING'>
+            job.status().eta
+            >> 43.241  # seconds
+        """
+        time = datetime.now()
+        cancelled = False
+        if self.communicator:
+            with self.communicator.lock:
+                cancelled = self.communicator.should_cancel
+        if cancelled:
+            return StatusUpdate(
+                code=Status.CANCELLED,
+                rank=0,
+                queue_size=None,
+                success=False,
+                time=time,
+                eta=None,
+            )
+        if self.done():
+            if not self.future._exception:  # type: ignore
+                return StatusUpdate(
+                    code=Status.FINISHED,
+                    rank=0,
+                    queue_size=None,
+                    success=True,
+                    time=time,
+                    eta=None,
+                )
+            else:
+                return StatusUpdate(
+                    code=Status.FINISHED,
+                    rank=0,
+                    queue_size=None,
+                    success=False,
+                    time=time,
+                    eta=None,
+                )
+        else:
+            if not self.communicator:
+                return StatusUpdate(
+                    code=Status.PROCESSING,
+                    rank=0,
+                    queue_size=None,
+                    success=None,
+                    time=time,
+                    eta=None,
+                )
+            else:
+                with self.communicator.lock:
+                    eta = self.communicator.job.latest_status.eta
+                    if self.verbose and self.space_id and eta and eta > 30:
+                        print(
+                            f"Due to heavy traffic on this app, the prediction will take approximately {int(eta)} seconds."
+                            f"For faster predictions without waiting in queue, you may duplicate the space using: Client.duplicate({self.space_id})"
+                        )
+                    return self.communicator.job.latest_status
+
+    def __getattr__(self, name):
+        """Forwards any properties to the Future class."""
+        return getattr(self.future, name)
+
+    def cancel(self) -> bool:
+        """Cancels the job as best as possible.
+
+        If the app you are connecting to has the gradio queue enabled, the job
+        will be cancelled locally as soon as possible. For apps that do not use the
+        queue, the job cannot be cancelled if it's been sent to the local executor
+        (for the time being).
+
+        Note: In general, this DOES not stop the process from running in the upstream server
+        except for the following situations:
+
+        1. If the job is queued upstream, it will be removed from the queue and the server will not run the job
+        2. If the job has iterative outputs, the job will finish as soon as the current iteration finishes running
+        3. If the job has not been picked up by the queue yet, the queue will not pick up the job
+        """
+        if self.communicator:
+            with self.communicator.lock:
+                self.communicator.should_cancel = True
+                return True
+        return self.future.cancel()
```

### Comparing `gradio_client-0.0.9/gradio_client/documentation.py` & `gradio_client-0.1.0/gradio_client/documentation.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,266 +1,266 @@
-"""Contains methods that generate documentation for Gradio functions and classes."""
-
-from __future__ import annotations
-
-import inspect
-from typing import Callable, Dict, List, Tuple
-
-classes_to_document = {}
-classes_inherit_documentation = {}
-documentation_group = None
-
-
-def set_documentation_group(m):
-    global documentation_group
-    documentation_group = m
-    if m not in classes_to_document:
-        classes_to_document[m] = []
-
-
-def extract_instance_attr_doc(cls, attr):
-    code = inspect.getsource(cls.__init__)
-    lines = [line.strip() for line in code.split("\n")]
-    i = None
-    for i, line in enumerate(lines):
-        if line.startswith("self." + attr + ":") or line.startswith(
-            "self." + attr + " ="
-        ):
-            break
-    assert i is not None, f"Could not find {attr} in {cls.__name__}"
-    start_line = lines.index('"""', i)
-    end_line = lines.index('"""', start_line + 1)
-    for j in range(i + 1, start_line):
-        assert not lines[j].startswith("self."), (
-            f"Found another attribute before docstring for {attr} in {cls.__name__}: "
-            + lines[j]
-            + "\n start:"
-            + lines[i]
-        )
-    doc_string = " ".join(lines[start_line + 1 : end_line])
-    return doc_string
-
-
-def document(*fns, inherit=False):
-    """
-    Defines the @document decorator which adds classes or functions to the Gradio
-    documentation at www.gradio.app/docs.
-
-    Usage examples:
-    - Put @document() above a class to document the class and its constructor.
-    - Put @document("fn1", "fn2") above a class to also document methods fn1 and fn2.
-    - Put @document("*fn3") with an asterisk above a class to document the instance attribute methods f3.
-    """
-
-    def inner_doc(cls):
-        global documentation_group
-        if inherit:
-            classes_inherit_documentation[cls] = None
-        classes_to_document[documentation_group].append((cls, fns))
-        return cls
-
-    return inner_doc
-
-
-def document_fn(fn: Callable, cls) -> Tuple[str, List[Dict], Dict, str | None]:
-    """
-    Generates documentation for any function.
-    Parameters:
-        fn: Function to document
-    Returns:
-        description: General description of fn
-        parameters: A list of dicts for each parameter, storing data for the parameter name, annotation and doc
-        return: A dict storing data for the returned annotation and doc
-        example: Code for an example use of the fn
-    """
-    doc_str = inspect.getdoc(fn) or ""
-    doc_lines = doc_str.split("\n")
-    signature = inspect.signature(fn)
-    description, parameters, returns, examples = [], {}, [], []
-    mode = "description"
-    for line in doc_lines:
-        line = line.rstrip()
-        if line == "Parameters:":
-            mode = "parameter"
-        elif line.startswith("Example:"):
-            mode = "example"
-            if "(" in line and ")" in line:
-                c = line.split("(")[1].split(")")[0]
-                if c != cls.__name__:
-                    mode = "ignore"
-        elif line == "Returns:":
-            mode = "return"
-        else:
-            if mode == "description":
-                description.append(line if line.strip() else "<br>")
-                continue
-            if not (line.startswith("    ") or line.strip() == ""):
-                print(line)
-            assert (
-                line.startswith("    ") or line.strip() == ""
-            ), f"Documentation format for {fn.__name__} has format error in line: {line}"
-            line = line[4:]
-            if mode == "parameter":
-                colon_index = line.index(": ")
-                assert (
-                    colon_index > -1
-                ), f"Documentation format for {fn.__name__} has format error in line: {line}"
-                parameter = line[:colon_index]
-                parameter_doc = line[colon_index + 2 :]
-                parameters[parameter] = parameter_doc
-            elif mode == "return":
-                returns.append(line)
-            elif mode == "example":
-                examples.append(line)
-    description_doc = " ".join(description)
-    parameter_docs = []
-    for param_name, param in signature.parameters.items():
-        if param_name.startswith("_"):
-            continue
-        if param_name in ["kwargs", "args"] and param_name not in parameters:
-            continue
-        parameter_doc = {
-            "name": param_name,
-            "annotation": param.annotation,
-            "doc": parameters.get(param_name),
-        }
-        if param_name in parameters:
-            del parameters[param_name]
-        if param.default != inspect.Parameter.empty:
-            default = param.default
-            if type(default) == str:
-                default = '"' + default + '"'
-            if default.__class__.__module__ != "builtins":
-                default = f"{default.__class__.__name__}()"
-            parameter_doc["default"] = default
-        elif parameter_doc["doc"] is not None:
-            if "kwargs" in parameter_doc["doc"]:
-                parameter_doc["kwargs"] = True
-            if "args" in parameter_doc["doc"]:
-                parameter_doc["args"] = True
-        parameter_docs.append(parameter_doc)
-    assert (
-        len(parameters) == 0
-    ), f"Documentation format for {fn.__name__} documents nonexistent parameters: {''.join(parameters.keys())}"
-    if len(returns) == 0:
-        return_docs = {}
-    elif len(returns) == 1:
-        return_docs = {"annotation": signature.return_annotation, "doc": returns[0]}
-    else:
-        return_docs = {}
-        # raise ValueError("Does not support multiple returns yet.")
-    examples_doc = "\n".join(examples) if len(examples) > 0 else None
-    return description_doc, parameter_docs, return_docs, examples_doc
-
-
-def document_cls(cls):
-    doc_str = inspect.getdoc(cls)
-    if doc_str is None:
-        return "", {}, ""
-    tags = {}
-    description_lines = []
-    mode = "description"
-    for line in doc_str.split("\n"):
-        line = line.rstrip()
-        if line.endswith(":") and " " not in line:
-            mode = line[:-1].lower()
-            tags[mode] = []
-        elif line.split(" ")[0].endswith(":") and not line.startswith("    "):
-            tag = line[: line.index(":")].lower()
-            value = line[line.index(":") + 2 :]
-            tags[tag] = value
-        else:
-            if mode == "description":
-                description_lines.append(line if line.strip() else "<br>")
-            else:
-                assert (
-                    line.startswith("    ") or not line.strip()
-                ), f"Documentation format for {cls.__name__} has format error in line: {line}"
-                tags[mode].append(line[4:])
-    if "example" in tags:
-        example = "\n".join(tags["example"])
-        del tags["example"]
-    else:
-        example = None
-    for key, val in tags.items():
-        if isinstance(val, list):
-            tags[key] = "<br>".join(val)
-    description = " ".join(description_lines).replace("\n", "<br>")
-    return description, tags, example
-
-
-def generate_documentation():
-    documentation = {}
-    for mode, class_list in classes_to_document.items():
-        documentation[mode] = []
-        for cls, fns in class_list:
-            fn_to_document = cls if inspect.isfunction(cls) else cls.__init__
-            _, parameter_doc, return_doc, _ = document_fn(fn_to_document, cls)
-            cls_description, cls_tags, cls_example = document_cls(cls)
-            cls_documentation = {
-                "class": cls,
-                "name": cls.__name__,
-                "description": cls_description,
-                "tags": cls_tags,
-                "parameters": parameter_doc,
-                "returns": return_doc,
-                "example": cls_example,
-                "fns": [],
-            }
-            for fn_name in fns:
-                instance_attribute_fn = fn_name.startswith("*")
-                if instance_attribute_fn:
-                    fn_name = fn_name[1:]
-                    # Instance attribute fns are classes
-                    # whose __call__ method determines their behavior
-                    fn = getattr(cls(), fn_name).__call__
-                else:
-                    fn = getattr(cls, fn_name)
-                if not callable(fn):
-                    description_doc = str(fn)
-                    parameter_docs = {}
-                    return_docs = {}
-                    examples_doc = ""
-                    override_signature = f"gr.{cls.__name__}.{fn_name}"
-                else:
-                    (
-                        description_doc,
-                        parameter_docs,
-                        return_docs,
-                        examples_doc,
-                    ) = document_fn(fn, cls)
-                    override_signature = None
-                if instance_attribute_fn:
-                    description_doc = extract_instance_attr_doc(cls, fn_name)
-                cls_documentation["fns"].append(
-                    {
-                        "fn": fn,
-                        "name": fn_name,
-                        "description": description_doc,
-                        "tags": {},
-                        "parameters": parameter_docs,
-                        "returns": return_docs,
-                        "example": examples_doc,
-                        "override_signature": override_signature,
-                    }
-                )
-            documentation[mode].append(cls_documentation)
-            if cls in classes_inherit_documentation:
-                classes_inherit_documentation[cls] = cls_documentation["fns"]
-    for mode, class_list in classes_to_document.items():
-        for i, (cls, _) in enumerate(class_list):
-            for super_class in classes_inherit_documentation:
-                if (
-                    inspect.isclass(cls)
-                    and issubclass(cls, super_class)
-                    and cls != super_class
-                ):
-                    for inherited_fn in classes_inherit_documentation[super_class]:
-                        inherited_fn = dict(inherited_fn)
-                        try:
-                            inherited_fn["description"] = extract_instance_attr_doc(
-                                cls, inherited_fn["name"]
-                            )
-                        except (ValueError, AssertionError):
-                            pass
-                        documentation[mode][i]["fns"].append(inherited_fn)
-    return documentation
+"""Contains methods that generate documentation for Gradio functions and classes."""
+
+from __future__ import annotations
+
+import inspect
+from typing import Callable, Dict, List, Tuple
+
+classes_to_document = {}
+classes_inherit_documentation = {}
+documentation_group = None
+
+
+def set_documentation_group(m):
+    global documentation_group
+    documentation_group = m
+    if m not in classes_to_document:
+        classes_to_document[m] = []
+
+
+def extract_instance_attr_doc(cls, attr):
+    code = inspect.getsource(cls.__init__)
+    lines = [line.strip() for line in code.split("\n")]
+    i = None
+    for i, line in enumerate(lines):
+        if line.startswith("self." + attr + ":") or line.startswith(
+            "self." + attr + " ="
+        ):
+            break
+    assert i is not None, f"Could not find {attr} in {cls.__name__}"
+    start_line = lines.index('"""', i)
+    end_line = lines.index('"""', start_line + 1)
+    for j in range(i + 1, start_line):
+        assert not lines[j].startswith("self."), (
+            f"Found another attribute before docstring for {attr} in {cls.__name__}: "
+            + lines[j]
+            + "\n start:"
+            + lines[i]
+        )
+    doc_string = " ".join(lines[start_line + 1 : end_line])
+    return doc_string
+
+
+def document(*fns, inherit=False):
+    """
+    Defines the @document decorator which adds classes or functions to the Gradio
+    documentation at www.gradio.app/docs.
+
+    Usage examples:
+    - Put @document() above a class to document the class and its constructor.
+    - Put @document("fn1", "fn2") above a class to also document methods fn1 and fn2.
+    - Put @document("*fn3") with an asterisk above a class to document the instance attribute methods f3.
+    """
+
+    def inner_doc(cls):
+        global documentation_group
+        if inherit:
+            classes_inherit_documentation[cls] = None
+        classes_to_document[documentation_group].append((cls, fns))
+        return cls
+
+    return inner_doc
+
+
+def document_fn(fn: Callable, cls) -> Tuple[str, List[Dict], Dict, str | None]:
+    """
+    Generates documentation for any function.
+    Parameters:
+        fn: Function to document
+    Returns:
+        description: General description of fn
+        parameters: A list of dicts for each parameter, storing data for the parameter name, annotation and doc
+        return: A dict storing data for the returned annotation and doc
+        example: Code for an example use of the fn
+    """
+    doc_str = inspect.getdoc(fn) or ""
+    doc_lines = doc_str.split("\n")
+    signature = inspect.signature(fn)
+    description, parameters, returns, examples = [], {}, [], []
+    mode = "description"
+    for line in doc_lines:
+        line = line.rstrip()
+        if line == "Parameters:":
+            mode = "parameter"
+        elif line.startswith("Example:"):
+            mode = "example"
+            if "(" in line and ")" in line:
+                c = line.split("(")[1].split(")")[0]
+                if c != cls.__name__:
+                    mode = "ignore"
+        elif line == "Returns:":
+            mode = "return"
+        else:
+            if mode == "description":
+                description.append(line if line.strip() else "<br>")
+                continue
+            if not (line.startswith("    ") or line.strip() == ""):
+                print(line)
+            assert (
+                line.startswith("    ") or line.strip() == ""
+            ), f"Documentation format for {fn.__name__} has format error in line: {line}"
+            line = line[4:]
+            if mode == "parameter":
+                colon_index = line.index(": ")
+                assert (
+                    colon_index > -1
+                ), f"Documentation format for {fn.__name__} has format error in line: {line}"
+                parameter = line[:colon_index]
+                parameter_doc = line[colon_index + 2 :]
+                parameters[parameter] = parameter_doc
+            elif mode == "return":
+                returns.append(line)
+            elif mode == "example":
+                examples.append(line)
+    description_doc = " ".join(description)
+    parameter_docs = []
+    for param_name, param in signature.parameters.items():
+        if param_name.startswith("_"):
+            continue
+        if param_name in ["kwargs", "args"] and param_name not in parameters:
+            continue
+        parameter_doc = {
+            "name": param_name,
+            "annotation": param.annotation,
+            "doc": parameters.get(param_name),
+        }
+        if param_name in parameters:
+            del parameters[param_name]
+        if param.default != inspect.Parameter.empty:
+            default = param.default
+            if type(default) == str:
+                default = '"' + default + '"'
+            if default.__class__.__module__ != "builtins":
+                default = f"{default.__class__.__name__}()"
+            parameter_doc["default"] = default
+        elif parameter_doc["doc"] is not None:
+            if "kwargs" in parameter_doc["doc"]:
+                parameter_doc["kwargs"] = True
+            if "args" in parameter_doc["doc"]:
+                parameter_doc["args"] = True
+        parameter_docs.append(parameter_doc)
+    assert (
+        len(parameters) == 0
+    ), f"Documentation format for {fn.__name__} documents nonexistent parameters: {''.join(parameters.keys())}"
+    if len(returns) == 0:
+        return_docs = {}
+    elif len(returns) == 1:
+        return_docs = {"annotation": signature.return_annotation, "doc": returns[0]}
+    else:
+        return_docs = {}
+        # raise ValueError("Does not support multiple returns yet.")
+    examples_doc = "\n".join(examples) if len(examples) > 0 else None
+    return description_doc, parameter_docs, return_docs, examples_doc
+
+
+def document_cls(cls):
+    doc_str = inspect.getdoc(cls)
+    if doc_str is None:
+        return "", {}, ""
+    tags = {}
+    description_lines = []
+    mode = "description"
+    for line in doc_str.split("\n"):
+        line = line.rstrip()
+        if line.endswith(":") and " " not in line:
+            mode = line[:-1].lower()
+            tags[mode] = []
+        elif line.split(" ")[0].endswith(":") and not line.startswith("    "):
+            tag = line[: line.index(":")].lower()
+            value = line[line.index(":") + 2 :]
+            tags[tag] = value
+        else:
+            if mode == "description":
+                description_lines.append(line if line.strip() else "<br>")
+            else:
+                assert (
+                    line.startswith("    ") or not line.strip()
+                ), f"Documentation format for {cls.__name__} has format error in line: {line}"
+                tags[mode].append(line[4:])
+    if "example" in tags:
+        example = "\n".join(tags["example"])
+        del tags["example"]
+    else:
+        example = None
+    for key, val in tags.items():
+        if isinstance(val, list):
+            tags[key] = "<br>".join(val)
+    description = " ".join(description_lines).replace("\n", "<br>")
+    return description, tags, example
+
+
+def generate_documentation():
+    documentation = {}
+    for mode, class_list in classes_to_document.items():
+        documentation[mode] = []
+        for cls, fns in class_list:
+            fn_to_document = cls if inspect.isfunction(cls) else cls.__init__
+            _, parameter_doc, return_doc, _ = document_fn(fn_to_document, cls)
+            cls_description, cls_tags, cls_example = document_cls(cls)
+            cls_documentation = {
+                "class": cls,
+                "name": cls.__name__,
+                "description": cls_description,
+                "tags": cls_tags,
+                "parameters": parameter_doc,
+                "returns": return_doc,
+                "example": cls_example,
+                "fns": [],
+            }
+            for fn_name in fns:
+                instance_attribute_fn = fn_name.startswith("*")
+                if instance_attribute_fn:
+                    fn_name = fn_name[1:]
+                    # Instance attribute fns are classes
+                    # whose __call__ method determines their behavior
+                    fn = getattr(cls(), fn_name).__call__
+                else:
+                    fn = getattr(cls, fn_name)
+                if not callable(fn):
+                    description_doc = str(fn)
+                    parameter_docs = {}
+                    return_docs = {}
+                    examples_doc = ""
+                    override_signature = f"gr.{cls.__name__}.{fn_name}"
+                else:
+                    (
+                        description_doc,
+                        parameter_docs,
+                        return_docs,
+                        examples_doc,
+                    ) = document_fn(fn, cls)
+                    override_signature = None
+                if instance_attribute_fn:
+                    description_doc = extract_instance_attr_doc(cls, fn_name)
+                cls_documentation["fns"].append(
+                    {
+                        "fn": fn,
+                        "name": fn_name,
+                        "description": description_doc,
+                        "tags": {},
+                        "parameters": parameter_docs,
+                        "returns": return_docs,
+                        "example": examples_doc,
+                        "override_signature": override_signature,
+                    }
+                )
+            documentation[mode].append(cls_documentation)
+            if cls in classes_inherit_documentation:
+                classes_inherit_documentation[cls] = cls_documentation["fns"]
+    for mode, class_list in classes_to_document.items():
+        for i, (cls, _) in enumerate(class_list):
+            for super_class in classes_inherit_documentation:
+                if (
+                    inspect.isclass(cls)
+                    and issubclass(cls, super_class)
+                    and cls != super_class
+                ):
+                    for inherited_fn in classes_inherit_documentation[super_class]:
+                        inherited_fn = dict(inherited_fn)
+                        try:
+                            inherited_fn["description"] = extract_instance_attr_doc(
+                                cls, inherited_fn["name"]
+                            )
+                        except (ValueError, AssertionError):
+                            pass
+                        documentation[mode][i]["fns"].append(inherited_fn)
+    return documentation
```

### Comparing `gradio_client-0.0.9/gradio_client/serializing.py` & `gradio_client-0.1.0/gradio_client/serializing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,420 +1,420 @@
-from __future__ import annotations
-
-import json
-import os
-import uuid
-from abc import ABC, abstractmethod
-from pathlib import Path
-from typing import Any, Dict, List, Tuple
-
-from gradio_client import utils
-from gradio_client.data_classes import FileData
-
-
-class Serializable(ABC):
-    @abstractmethod
-    def input_api_info(self) -> Tuple[str, str]:
-        """
-        Get the type of input that should be provided via API, and a human-readable description of the input as a tuple (for documentation generation).
-        """
-        pass
-
-    @abstractmethod
-    def output_api_info(self) -> Tuple[str, str]:
-        """
-        Get the type of output that should be returned via API, and a human-readable description of the output as a tuple (for documentation generation).
-        """
-        pass
-
-    def serialize(self, x: Any, load_dir: str | Path = ""):
-        """
-        Convert data from human-readable format to serialized format for a browser.
-        """
-        return x
-
-    def deserialize(
-        self,
-        x: Any,
-        save_dir: str | Path | None = None,
-        root_url: str | None = None,
-        hf_token: str | None = None,
-    ):
-        """
-        Convert data from serialized format for a browser to human-readable format.
-        """
-        return x
-
-
-class SimpleSerializable(Serializable):
-    """General class that does not perform any serialization or deserialization."""
-
-    def input_api_info(self) -> Tuple[str, str]:
-        return "Any", ""
-
-    def output_api_info(self) -> Tuple[str, str]:
-        return "Any", ""
-
-
-class StringSerializable(Serializable):
-    """Expects a string as input/output but performs no serialization."""
-
-    def input_api_info(self) -> Tuple[str, str]:
-        return "str", "value"
-
-    def output_api_info(self) -> Tuple[str, str]:
-        return "str", "value"
-
-
-class ListStringSerializable(Serializable):
-    """Expects a list of strings as input/output but performs no serialization."""
-
-    def input_api_info(self) -> Tuple[str, str]:
-        return "List[str]", "values"
-
-    def output_api_info(self) -> Tuple[str, str]:
-        return "List[str]", "values"
-
-
-class BooleanSerializable(Serializable):
-    """Expects a boolean as input/output but performs no serialization."""
-
-    def input_api_info(self) -> Tuple[str, str]:
-        return "bool", "value"
-
-    def output_api_info(self) -> Tuple[str, str]:
-        return "bool", "value"
-
-
-class NumberSerializable(Serializable):
-    """Expects a number (int/float) as input/output but performs no serialization."""
-
-    def input_api_info(self) -> Tuple[str, str]:
-        return "int | float", "value"
-
-    def output_api_info(self) -> Tuple[str, str]:
-        return "int | float", "value"
-
-
-class ImgSerializable(Serializable):
-    """Expects a base64 string as input/output which is ."""
-
-    def input_api_info(self) -> Tuple[str, str]:
-        return "str", "filepath or URL"
-
-    def output_api_info(self) -> Tuple[str, str]:
-        return "str", "filepath or URL"
-
-    def serialize(
-        self,
-        x: str | None,
-        load_dir: str | Path = "",
-    ) -> str | None:
-        """
-        Convert from human-friendly version of a file (string filepath) to a seralized
-        representation (base64).
-        Parameters:
-            x: String path to file to serialize
-            load_dir: Path to directory containing x
-        """
-        if x is None or x == "":
-            return None
-        is_url = utils.is_valid_url(x)
-        path = x if is_url else Path(load_dir) / x
-        return utils.encode_url_or_file_to_base64(path)
-
-    def deserialize(
-        self,
-        x: str | None,
-        save_dir: str | Path | None = None,
-        root_url: str | None = None,
-        hf_token: str | None = None,
-    ) -> str | None:
-        """
-        Convert from serialized representation of a file (base64) to a human-friendly
-        version (string filepath). Optionally, save the file to the directory specified by save_dir
-        Parameters:
-            x: Base64 representation of image to deserialize into a string filepath
-            save_dir: Path to directory to save the deserialized image to
-            root_url: Ignored
-            hf_token: Ignored
-        """
-        if x is None or x == "":
-            return None
-        file = utils.decode_base64_to_file(x, dir=save_dir)
-        return file.name
-
-
-class FileSerializable(Serializable):
-    def input_api_info(self) -> Tuple[str, str]:
-        return "str", "filepath or URL"
-
-    def output_api_info(self) -> Tuple[str, str]:
-        return "str", "filepath or URL"
-
-    def _serialize_single(
-        self, x: str | FileData | None, load_dir: str | Path = ""
-    ) -> FileData | None:
-        if x is None or isinstance(x, dict):
-            return x
-        if utils.is_valid_url(x):
-            filename = x
-            size = None
-        else:
-            filename = str(Path(load_dir) / x)
-            size = Path(filename).stat().st_size
-        return {
-            "name": filename,
-            "data": utils.encode_url_or_file_to_base64(filename),
-            "orig_name": Path(filename).name,
-            "is_file": False,
-            "size": size,
-        }
-
-    def _deserialize_single(
-        self,
-        x: str | FileData | None,
-        save_dir: str | None = None,
-        root_url: str | None = None,
-        hf_token: str | None = None,
-    ) -> str | None:
-        if x is None:
-            return None
-        if isinstance(x, str):
-            file_name = utils.decode_base64_to_file(x, dir=save_dir).name
-        elif isinstance(x, dict):
-            if x.get("is_file", False):
-                filepath = x.get("name")
-                assert filepath is not None, f"The 'name' field is missing in {x}"
-                if root_url is not None:
-                    file_name = utils.download_tmp_copy_of_file(
-                        root_url + "file=" + filepath,
-                        hf_token=hf_token,
-                        dir=save_dir,
-                    ).name
-                else:
-                    file_name = utils.create_tmp_copy_of_file(
-                        filepath, dir=save_dir
-                    ).name
-            else:
-                file_name = utils.decode_base64_to_file(x["data"], dir=save_dir).name
-        else:
-            raise ValueError(
-                f"A FileSerializable component can only deserialize a string or a dict, not a {type(x)}: {x}"
-            )
-        return file_name
-
-    def serialize(
-        self,
-        x: str | FileData | None | List[str | FileData | None],
-        load_dir: str | Path = "",
-    ) -> FileData | None | List[FileData | None]:
-        """
-        Convert from human-friendly version of a file (string filepath) to a
-        seralized representation (base64)
-        Parameters:
-            x: String path to file to serialize
-            load_dir: Path to directory containing x
-        """
-        if x is None or x == "":
-            return None
-        if isinstance(x, list):
-            return [self._serialize_single(f, load_dir=load_dir) for f in x]
-        else:
-            return self._serialize_single(x, load_dir=load_dir)
-
-    def deserialize(
-        self,
-        x: str | FileData | None | List[str | FileData | None],
-        save_dir: Path | str | None = None,
-        root_url: str | None = None,
-        hf_token: str | None = None,
-    ) -> str | None | List[str | None]:
-        """
-        Convert from serialized representation of a file (base64) to a human-friendly
-        version (string filepath). Optionally, save the file to the directory specified by `save_dir`
-        Parameters:
-            x: Base64 representation of file to deserialize into a string filepath
-            save_dir: Path to directory to save the deserialized file to
-            root_url: If this component is loaded from an external Space, this is the URL of the Space.
-            hf_token: If this component is loaded from an external private Space, this is the access token for the Space
-        """
-        if x is None:
-            return None
-        if isinstance(save_dir, Path):
-            save_dir = str(save_dir)
-        if isinstance(x, list):
-            return [
-                self._deserialize_single(
-                    f, save_dir=save_dir, root_url=root_url, hf_token=hf_token
-                )
-                for f in x
-            ]
-        else:
-            return self._deserialize_single(
-                x, save_dir=save_dir, root_url=root_url, hf_token=hf_token
-            )
-
-
-class VideoSerializable(FileSerializable):
-    def input_api_info(self) -> Tuple[str, str]:
-        return "str", "Filepath or URL to a video file"
-
-    def output_api_info(self) -> Tuple[str, str]:
-        return (
-            "str | Tuple[str, str]",
-            "Filepath or URL to a video file, or a tuple of (video file, subtitle file)",
-        )
-
-    def serialize(
-        self, x: str | None, load_dir: str | Path = ""
-    ) -> Tuple[FileData | None, None]:
-        return (super().serialize(x, load_dir), None)  # type: ignore
-
-    def deserialize(
-        self,
-        x: Tuple[FileData | None, FileData | None] | None,
-        save_dir: Path | str | None = None,
-        root_url: str | None = None,
-        hf_token: str | None = None,
-    ) -> str | Tuple[str | None, str | None] | None:
-        """
-        Convert from serialized representation of a file (base64) to a human-friendly
-        version (string filepath). Optionally, save the file to the directory specified by `save_dir`
-        """
-        if isinstance(x, tuple):
-            assert len(x) == 2, f"Expected tuple of length 2. Received: {x}"
-            x_as_list = [x[0], x[1]]
-        else:
-            raise ValueError(f"Expected tuple of length 2. Received: {x}")
-        deserialized_file = super().deserialize(x_as_list, save_dir, root_url, hf_token)
-        if isinstance(deserialized_file, list):
-            return deserialized_file[0]  # ignore subtitles
-
-
-class JSONSerializable(Serializable):
-    def input_api_info(self) -> Tuple[str, str]:
-        return "str", "filepath to json file"
-
-    def output_api_info(self) -> Tuple[str, str]:
-        return "str", "filepath to json file"
-
-    def serialize(
-        self,
-        x: str | None,
-        load_dir: str | Path = "",
-    ) -> Dict | None:
-        """
-        Convert from a a human-friendly version (string path to json file) to a
-        serialized representation (json string)
-        Parameters:
-            x: String path to json file to read to get json string
-            load_dir: Path to directory containing x
-        """
-        if x is None or x == "":
-            return None
-        return utils.file_to_json(Path(load_dir) / x)
-
-    def deserialize(
-        self,
-        x: str | Dict,
-        save_dir: str | Path | None = None,
-        root_url: str | None = None,
-        hf_token: str | None = None,
-    ) -> str | None:
-        """
-        Convert from serialized representation (json string) to a human-friendly
-        version (string path to json file).  Optionally, save the file to the directory specified by `save_dir`
-        Parameters:
-            x: Json string
-            save_dir: Path to save the deserialized json file to
-            root_url: Ignored
-            hf_token: Ignored
-        """
-        if x is None:
-            return None
-        return utils.dict_or_str_to_json_file(x, dir=save_dir).name
-
-
-class GallerySerializable(Serializable):
-    def input_api_info(self) -> Tuple[str, str]:
-        return "str", "path to directory with images and captions.json"
-
-    def output_api_info(self) -> Tuple[str, str]:
-        return "str", "path to directory with images and captions.json"
-
-    def serialize(
-        self, x: str | None, load_dir: str | Path = ""
-    ) -> List[List[str]] | None:
-        if x is None or x == "":
-            return None
-        files = []
-        captions_file = Path(x) / "captions.json"
-        with captions_file.open("r") as captions_json:
-            captions = json.load(captions_json)
-        for file_name, caption in captions.items():
-            img = FileSerializable().serialize(file_name)
-            files.append([img, caption])
-        return files
-
-    def deserialize(
-        self,
-        x: Any,
-        save_dir: str = "",
-        root_url: str | None = None,
-        hf_token: str | None = None,
-    ) -> None | str:
-        if x is None:
-            return None
-        gallery_path = Path(save_dir) / str(uuid.uuid4())
-        gallery_path.mkdir(exist_ok=True, parents=True)
-        captions = {}
-        for img_data in x:
-            if isinstance(img_data, list) or isinstance(img_data, tuple):
-                img_data, caption = img_data
-            else:
-                caption = None
-            name = FileSerializable().deserialize(
-                img_data, gallery_path, root_url=root_url, hf_token=hf_token
-            )
-            captions[name] = caption
-            captions_file = gallery_path / "captions.json"
-            with captions_file.open("w") as captions_json:
-                json.dump(captions, captions_json)
-        return os.path.abspath(gallery_path)
-
-
-SERIALIZER_MAPPING = {cls.__name__: cls for cls in Serializable.__subclasses__()}
-SERIALIZER_MAPPING["Serializable"] = SimpleSerializable
-SERIALIZER_MAPPING["File"] = FileSerializable
-SERIALIZER_MAPPING["UploadButton"] = FileSerializable
-
-COMPONENT_MAPPING: Dict[str, type] = {
-    "textbox": StringSerializable,
-    "number": NumberSerializable,
-    "slider": NumberSerializable,
-    "checkbox": BooleanSerializable,
-    "checkboxgroup": ListStringSerializable,
-    "radio": StringSerializable,
-    "dropdown": SimpleSerializable,
-    "image": ImgSerializable,
-    "video": FileSerializable,
-    "audio": FileSerializable,
-    "file": FileSerializable,
-    "dataframe": JSONSerializable,
-    "timeseries": JSONSerializable,
-    "state": SimpleSerializable,
-    "button": StringSerializable,
-    "uploadbutton": FileSerializable,
-    "colorpicker": StringSerializable,
-    "label": JSONSerializable,
-    "highlightedtext": JSONSerializable,
-    "json": JSONSerializable,
-    "html": StringSerializable,
-    "gallery": GallerySerializable,
-    "chatbot": JSONSerializable,
-    "model3d": FileSerializable,
-    "plot": JSONSerializable,
-    "markdown": StringSerializable,
-    "dataset": StringSerializable,
-    "code": StringSerializable,
-}
+from __future__ import annotations
+
+import json
+import os
+import uuid
+from abc import ABC, abstractmethod
+from pathlib import Path
+from typing import Any, Dict, List, Tuple
+
+from gradio_client import utils
+from gradio_client.data_classes import FileData
+
+
+class Serializable(ABC):
+    @abstractmethod
+    def input_api_info(self) -> Tuple[str, str]:
+        """
+        Get the type of input that should be provided via API, and a human-readable description of the input as a tuple (for documentation generation).
+        """
+        pass
+
+    @abstractmethod
+    def output_api_info(self) -> Tuple[str, str]:
+        """
+        Get the type of output that should be returned via API, and a human-readable description of the output as a tuple (for documentation generation).
+        """
+        pass
+
+    def serialize(self, x: Any, load_dir: str | Path = ""):
+        """
+        Convert data from human-readable format to serialized format for a browser.
+        """
+        return x
+
+    def deserialize(
+        self,
+        x: Any,
+        save_dir: str | Path | None = None,
+        root_url: str | None = None,
+        hf_token: str | None = None,
+    ):
+        """
+        Convert data from serialized format for a browser to human-readable format.
+        """
+        return x
+
+
+class SimpleSerializable(Serializable):
+    """General class that does not perform any serialization or deserialization."""
+
+    def input_api_info(self) -> Tuple[str, str]:
+        return "Any", ""
+
+    def output_api_info(self) -> Tuple[str, str]:
+        return "Any", ""
+
+
+class StringSerializable(Serializable):
+    """Expects a string as input/output but performs no serialization."""
+
+    def input_api_info(self) -> Tuple[str, str]:
+        return "str", "value"
+
+    def output_api_info(self) -> Tuple[str, str]:
+        return "str", "value"
+
+
+class ListStringSerializable(Serializable):
+    """Expects a list of strings as input/output but performs no serialization."""
+
+    def input_api_info(self) -> Tuple[str, str]:
+        return "List[str]", "values"
+
+    def output_api_info(self) -> Tuple[str, str]:
+        return "List[str]", "values"
+
+
+class BooleanSerializable(Serializable):
+    """Expects a boolean as input/output but performs no serialization."""
+
+    def input_api_info(self) -> Tuple[str, str]:
+        return "bool", "value"
+
+    def output_api_info(self) -> Tuple[str, str]:
+        return "bool", "value"
+
+
+class NumberSerializable(Serializable):
+    """Expects a number (int/float) as input/output but performs no serialization."""
+
+    def input_api_info(self) -> Tuple[str, str]:
+        return "int | float", "value"
+
+    def output_api_info(self) -> Tuple[str, str]:
+        return "int | float", "value"
+
+
+class ImgSerializable(Serializable):
+    """Expects a base64 string as input/output which is ."""
+
+    def input_api_info(self) -> Tuple[str, str]:
+        return "str", "filepath or URL"
+
+    def output_api_info(self) -> Tuple[str, str]:
+        return "str", "filepath or URL"
+
+    def serialize(
+        self,
+        x: str | None,
+        load_dir: str | Path = "",
+    ) -> str | None:
+        """
+        Convert from human-friendly version of a file (string filepath) to a seralized
+        representation (base64).
+        Parameters:
+            x: String path to file to serialize
+            load_dir: Path to directory containing x
+        """
+        if x is None or x == "":
+            return None
+        is_url = utils.is_valid_url(x)
+        path = x if is_url else Path(load_dir) / x
+        return utils.encode_url_or_file_to_base64(path)
+
+    def deserialize(
+        self,
+        x: str | None,
+        save_dir: str | Path | None = None,
+        root_url: str | None = None,
+        hf_token: str | None = None,
+    ) -> str | None:
+        """
+        Convert from serialized representation of a file (base64) to a human-friendly
+        version (string filepath). Optionally, save the file to the directory specified by save_dir
+        Parameters:
+            x: Base64 representation of image to deserialize into a string filepath
+            save_dir: Path to directory to save the deserialized image to
+            root_url: Ignored
+            hf_token: Ignored
+        """
+        if x is None or x == "":
+            return None
+        file = utils.decode_base64_to_file(x, dir=save_dir)
+        return file.name
+
+
+class FileSerializable(Serializable):
+    def input_api_info(self) -> Tuple[str, str]:
+        return "str", "filepath or URL"
+
+    def output_api_info(self) -> Tuple[str, str]:
+        return "str", "filepath or URL"
+
+    def _serialize_single(
+        self, x: str | FileData | None, load_dir: str | Path = ""
+    ) -> FileData | None:
+        if x is None or isinstance(x, dict):
+            return x
+        if utils.is_valid_url(x):
+            filename = x
+            size = None
+        else:
+            filename = str(Path(load_dir) / x)
+            size = Path(filename).stat().st_size
+        return {
+            "name": filename,
+            "data": utils.encode_url_or_file_to_base64(filename),
+            "orig_name": Path(filename).name,
+            "is_file": False,
+            "size": size,
+        }
+
+    def _deserialize_single(
+        self,
+        x: str | FileData | None,
+        save_dir: str | None = None,
+        root_url: str | None = None,
+        hf_token: str | None = None,
+    ) -> str | None:
+        if x is None:
+            return None
+        if isinstance(x, str):
+            file_name = utils.decode_base64_to_file(x, dir=save_dir).name
+        elif isinstance(x, dict):
+            if x.get("is_file", False):
+                filepath = x.get("name")
+                assert filepath is not None, f"The 'name' field is missing in {x}"
+                if root_url is not None:
+                    file_name = utils.download_tmp_copy_of_file(
+                        root_url + "file=" + filepath,
+                        hf_token=hf_token,
+                        dir=save_dir,
+                    ).name
+                else:
+                    file_name = utils.create_tmp_copy_of_file(
+                        filepath, dir=save_dir
+                    ).name
+            else:
+                file_name = utils.decode_base64_to_file(x["data"], dir=save_dir).name
+        else:
+            raise ValueError(
+                f"A FileSerializable component can only deserialize a string or a dict, not a {type(x)}: {x}"
+            )
+        return file_name
+
+    def serialize(
+        self,
+        x: str | FileData | None | List[str | FileData | None],
+        load_dir: str | Path = "",
+    ) -> FileData | None | List[FileData | None]:
+        """
+        Convert from human-friendly version of a file (string filepath) to a
+        seralized representation (base64)
+        Parameters:
+            x: String path to file to serialize
+            load_dir: Path to directory containing x
+        """
+        if x is None or x == "":
+            return None
+        if isinstance(x, list):
+            return [self._serialize_single(f, load_dir=load_dir) for f in x]
+        else:
+            return self._serialize_single(x, load_dir=load_dir)
+
+    def deserialize(
+        self,
+        x: str | FileData | None | List[str | FileData | None],
+        save_dir: Path | str | None = None,
+        root_url: str | None = None,
+        hf_token: str | None = None,
+    ) -> str | None | List[str | None]:
+        """
+        Convert from serialized representation of a file (base64) to a human-friendly
+        version (string filepath). Optionally, save the file to the directory specified by `save_dir`
+        Parameters:
+            x: Base64 representation of file to deserialize into a string filepath
+            save_dir: Path to directory to save the deserialized file to
+            root_url: If this component is loaded from an external Space, this is the URL of the Space.
+            hf_token: If this component is loaded from an external private Space, this is the access token for the Space
+        """
+        if x is None:
+            return None
+        if isinstance(save_dir, Path):
+            save_dir = str(save_dir)
+        if isinstance(x, list):
+            return [
+                self._deserialize_single(
+                    f, save_dir=save_dir, root_url=root_url, hf_token=hf_token
+                )
+                for f in x
+            ]
+        else:
+            return self._deserialize_single(
+                x, save_dir=save_dir, root_url=root_url, hf_token=hf_token
+            )
+
+
+class VideoSerializable(FileSerializable):
+    def input_api_info(self) -> Tuple[str, str]:
+        return "str", "Filepath or URL to a video file"
+
+    def output_api_info(self) -> Tuple[str, str]:
+        return (
+            "str | Tuple[str, str]",
+            "Filepath or URL to a video file, or a tuple of (video file, subtitle file)",
+        )
+
+    def serialize(
+        self, x: str | None, load_dir: str | Path = ""
+    ) -> Tuple[FileData | None, None]:
+        return (super().serialize(x, load_dir), None)  # type: ignore
+
+    def deserialize(
+        self,
+        x: Tuple[FileData | None, FileData | None] | None,
+        save_dir: Path | str | None = None,
+        root_url: str | None = None,
+        hf_token: str | None = None,
+    ) -> str | Tuple[str | None, str | None] | None:
+        """
+        Convert from serialized representation of a file (base64) to a human-friendly
+        version (string filepath). Optionally, save the file to the directory specified by `save_dir`
+        """
+        if isinstance(x, tuple):
+            assert len(x) == 2, f"Expected tuple of length 2. Received: {x}"
+            x_as_list = [x[0], x[1]]
+        else:
+            raise ValueError(f"Expected tuple of length 2. Received: {x}")
+        deserialized_file = super().deserialize(x_as_list, save_dir, root_url, hf_token)  # type: ignore
+        if isinstance(deserialized_file, list):
+            return deserialized_file[0]  # ignore subtitles
+
+
+class JSONSerializable(Serializable):
+    def input_api_info(self) -> Tuple[str, str]:
+        return "str", "filepath to json file"
+
+    def output_api_info(self) -> Tuple[str, str]:
+        return "str", "filepath to json file"
+
+    def serialize(
+        self,
+        x: str | None,
+        load_dir: str | Path = "",
+    ) -> Dict | None:
+        """
+        Convert from a a human-friendly version (string path to json file) to a
+        serialized representation (json string)
+        Parameters:
+            x: String path to json file to read to get json string
+            load_dir: Path to directory containing x
+        """
+        if x is None or x == "":
+            return None
+        return utils.file_to_json(Path(load_dir) / x)
+
+    def deserialize(
+        self,
+        x: str | Dict,
+        save_dir: str | Path | None = None,
+        root_url: str | None = None,
+        hf_token: str | None = None,
+    ) -> str | None:
+        """
+        Convert from serialized representation (json string) to a human-friendly
+        version (string path to json file).  Optionally, save the file to the directory specified by `save_dir`
+        Parameters:
+            x: Json string
+            save_dir: Path to save the deserialized json file to
+            root_url: Ignored
+            hf_token: Ignored
+        """
+        if x is None:
+            return None
+        return utils.dict_or_str_to_json_file(x, dir=save_dir).name
+
+
+class GallerySerializable(Serializable):
+    def input_api_info(self) -> Tuple[str, str]:
+        return "str", "path to directory with images and captions.json"
+
+    def output_api_info(self) -> Tuple[str, str]:
+        return "str", "path to directory with images and captions.json"
+
+    def serialize(
+        self, x: str | None, load_dir: str | Path = ""
+    ) -> List[List[str]] | None:
+        if x is None or x == "":
+            return None
+        files = []
+        captions_file = Path(x) / "captions.json"
+        with captions_file.open("r") as captions_json:
+            captions = json.load(captions_json)
+        for file_name, caption in captions.items():
+            img = FileSerializable().serialize(file_name)
+            files.append([img, caption])
+        return files
+
+    def deserialize(
+        self,
+        x: Any,
+        save_dir: str = "",
+        root_url: str | None = None,
+        hf_token: str | None = None,
+    ) -> None | str:
+        if x is None:
+            return None
+        gallery_path = Path(save_dir) / str(uuid.uuid4())
+        gallery_path.mkdir(exist_ok=True, parents=True)
+        captions = {}
+        for img_data in x:
+            if isinstance(img_data, list) or isinstance(img_data, tuple):
+                img_data, caption = img_data
+            else:
+                caption = None
+            name = FileSerializable().deserialize(
+                img_data, gallery_path, root_url=root_url, hf_token=hf_token
+            )
+            captions[name] = caption
+            captions_file = gallery_path / "captions.json"
+            with captions_file.open("w") as captions_json:
+                json.dump(captions, captions_json)
+        return os.path.abspath(gallery_path)
+
+
+SERIALIZER_MAPPING = {cls.__name__: cls for cls in Serializable.__subclasses__()}
+SERIALIZER_MAPPING["Serializable"] = SimpleSerializable
+SERIALIZER_MAPPING["File"] = FileSerializable
+SERIALIZER_MAPPING["UploadButton"] = FileSerializable
+
+COMPONENT_MAPPING: Dict[str, type] = {
+    "textbox": StringSerializable,
+    "number": NumberSerializable,
+    "slider": NumberSerializable,
+    "checkbox": BooleanSerializable,
+    "checkboxgroup": ListStringSerializable,
+    "radio": StringSerializable,
+    "dropdown": SimpleSerializable,
+    "image": ImgSerializable,
+    "video": FileSerializable,
+    "audio": FileSerializable,
+    "file": FileSerializable,
+    "dataframe": JSONSerializable,
+    "timeseries": JSONSerializable,
+    "state": SimpleSerializable,
+    "button": StringSerializable,
+    "uploadbutton": FileSerializable,
+    "colorpicker": StringSerializable,
+    "label": JSONSerializable,
+    "highlightedtext": JSONSerializable,
+    "json": JSONSerializable,
+    "html": StringSerializable,
+    "gallery": GallerySerializable,
+    "chatbot": JSONSerializable,
+    "model3d": FileSerializable,
+    "plot": JSONSerializable,
+    "markdown": StringSerializable,
+    "dataset": StringSerializable,
+    "code": StringSerializable,
+}
```

### Comparing `gradio_client-0.0.9/gradio_client/utils.py` & `gradio_client-0.1.0/gradio_client/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,397 +1,428 @@
-from __future__ import annotations
-
-import asyncio
-import base64
-import json
-import mimetypes
-import os
-import pkgutil
-import shutil
-import tempfile
-from concurrent.futures import CancelledError
-from dataclasses import dataclass, field
-from datetime import datetime
-from enum import Enum
-from pathlib import Path
-from threading import Lock
-from typing import Any, Callable, Dict, List, Tuple
-
-import fsspec.asyn
-import httpx
-import requests
-from websockets.legacy.protocol import WebSocketCommonProtocol
-
-API_URL = "/api/predict/"
-WS_URL = "/queue/join"
-UPLOAD_URL = "/upload"
-RESET_URL = "/reset"
-DUPLICATE_URL = "https://huggingface.co/spaces/{}?duplicate=true"
-STATE_COMPONENT = "state"
-
-__version__ = (pkgutil.get_data(__name__, "version.txt") or b"").decode("ascii").strip()
-
-
-class TooManyRequestsError(Exception):
-    """Raised when the API returns a 429 status code."""
-
-    pass
-
-
-class QueueError(Exception):
-    """Raised when the queue is full or there is an issue adding a job to the queue."""
-
-    pass
-
-
-class InvalidAPIEndpointError(Exception):
-    """Raised when the API endpoint is invalid."""
-
-    pass
-
-
-class Status(Enum):
-    """Status codes presented to client users."""
-
-    STARTING = "STARTING"
-    JOINING_QUEUE = "JOINING_QUEUE"
-    QUEUE_FULL = "QUEUE_FULL"
-    IN_QUEUE = "IN_QUEUE"
-    SENDING_DATA = "SENDING_DATA"
-    PROCESSING = "PROCESSSING"
-    ITERATING = "ITERATING"
-    FINISHED = "FINISHED"
-    CANCELLED = "CANCELLED"
-
-    @staticmethod
-    def ordering(status: "Status") -> int:
-        """Order of messages. Helpful for testing."""
-        order = [
-            Status.STARTING,
-            Status.JOINING_QUEUE,
-            Status.QUEUE_FULL,
-            Status.IN_QUEUE,
-            Status.SENDING_DATA,
-            Status.PROCESSING,
-            Status.ITERATING,
-            Status.FINISHED,
-            Status.CANCELLED,
-        ]
-        return order.index(status)
-
-    def __lt__(self, other: "Status"):
-        return self.ordering(self) < self.ordering(other)
-
-    @staticmethod
-    def msg_to_status(msg: str) -> "Status":
-        """Map the raw message from the backend to the status code presented to users."""
-        return {
-            "send_hash": Status.JOINING_QUEUE,
-            "queue_full": Status.QUEUE_FULL,
-            "estimation": Status.IN_QUEUE,
-            "send_data": Status.SENDING_DATA,
-            "process_starts": Status.PROCESSING,
-            "process_generating": Status.ITERATING,
-            "process_completed": Status.FINISHED,
-        }[msg]
-
-
-@dataclass
-class StatusUpdate:
-    """Update message sent from the worker thread to the Job on the main thread."""
-
-    code: Status
-    rank: int | None
-    queue_size: int | None
-    eta: float | None
-    success: bool | None
-    time: datetime | None
-
-
-def create_initial_status_update():
-    return StatusUpdate(
-        code=Status.STARTING,
-        rank=None,
-        queue_size=None,
-        eta=None,
-        success=None,
-        time=datetime.now(),
-    )
-
-
-@dataclass
-class JobStatus:
-    """The job status.
-
-    Keeps strack of the latest status update and intermediate outputs (not yet implements).
-    """
-
-    latest_status: StatusUpdate = field(default_factory=create_initial_status_update)
-    outputs: List[Any] = field(default_factory=list)
-
-
-@dataclass
-class Communicator:
-    """Helper class to help communicate between the worker thread and main thread."""
-
-    lock: Lock
-    job: JobStatus
-    deserialize: Callable[..., Tuple]
-    reset_url: str
-    should_cancel: bool = False
-
-
-########################
-# Network utils
-########################
-
-
-def is_valid_url(possible_url: str) -> bool:
-    headers = {"User-Agent": "gradio (https://gradio.app/; team@gradio.app)"}
-    try:
-        head_request = requests.head(possible_url, headers=headers)
-        if head_request.status_code == 405:
-            return requests.get(possible_url, headers=headers).ok
-        return head_request.ok
-    except Exception:
-        return False
-
-
-async def get_pred_from_ws(
-    websocket: WebSocketCommonProtocol,
-    data: str,
-    hash_data: str,
-    helper: Communicator | None = None,
-) -> Dict[str, Any]:
-    completed = False
-    resp = {}
-    while not completed:
-        # Receive message in the background so that we can
-        # cancel even while running a long pred
-        task = asyncio.create_task(websocket.recv())
-        while not task.done():
-            if helper:
-                with helper.lock:
-                    if helper.should_cancel:
-                        # Need to reset the iterator state since the client
-                        # will not reset the session
-                        async with httpx.AsyncClient() as http:
-                            reset = http.post(
-                                helper.reset_url, json=json.loads(hash_data)
-                            )
-                            # Retrieve cancel exception from task
-                            # otherwise will get nasty warning in console
-                            task.cancel()
-                            await asyncio.gather(task, reset, return_exceptions=True)
-                        raise CancelledError()
-            # Need to suspend this coroutine so that task actually runs
-            await asyncio.sleep(0.01)
-        msg = task.result()
-        resp = json.loads(msg)
-        if helper:
-            with helper.lock:
-                status_update = StatusUpdate(
-                    code=Status.msg_to_status(resp["msg"]),
-                    queue_size=resp.get("queue_size"),
-                    rank=resp.get("rank", None),
-                    success=resp.get("success"),
-                    time=datetime.now(),
-                    eta=resp.get("rank_eta"),
-                )
-                output = resp.get("output", {}).get("data", [])
-                if output and status_update.code != Status.FINISHED:
-                    try:
-                        result = helper.deserialize(*output)
-                    except Exception as e:
-                        result = [e]
-                    helper.job.outputs.append(result)
-                helper.job.latest_status = status_update
-        if resp["msg"] == "queue_full":
-            raise QueueError("Queue is full! Please try again.")
-        if resp["msg"] == "send_hash":
-            await websocket.send(hash_data)
-        elif resp["msg"] == "send_data":
-            await websocket.send(data)
-        completed = resp["msg"] == "process_completed"
-    return resp["output"]
-
-
-########################
-# Data processing utils
-########################
-
-
-def download_tmp_copy_of_file(
-    url_path: str, hf_token: str | None = None, dir: str | None = None
-) -> tempfile._TemporaryFileWrapper:
-    if dir is not None:
-        os.makedirs(dir, exist_ok=True)
-    headers = {"Authorization": "Bearer " + hf_token} if hf_token else {}
-    prefix = Path(url_path).stem
-    suffix = Path(url_path).suffix
-    file_obj = tempfile.NamedTemporaryFile(
-        delete=False,
-        prefix=prefix,
-        suffix=suffix,
-        dir=dir,
-    )
-    with requests.get(url_path, headers=headers, stream=True) as r:
-        with open(file_obj.name, "wb") as f:
-            shutil.copyfileobj(r.raw, f)
-    return file_obj
-
-
-def create_tmp_copy_of_file(
-    file_path: str, dir: str | None = None
-) -> tempfile._TemporaryFileWrapper:
-    if dir is not None:
-        os.makedirs(dir, exist_ok=True)
-    prefix = Path(file_path).stem
-    suffix = Path(file_path).suffix
-    file_obj = tempfile.NamedTemporaryFile(
-        delete=False,
-        prefix=prefix,
-        suffix=suffix,
-        dir=dir,
-    )
-    shutil.copy2(file_path, file_obj.name)
-    return file_obj
-
-
-def get_mimetype(filename: str) -> str | None:
-    mimetype = mimetypes.guess_type(filename)[0]
-    if mimetype is not None:
-        mimetype = mimetype.replace("x-wav", "wav").replace("x-flac", "flac")
-    return mimetype
-
-
-def get_extension(encoding: str) -> str | None:
-    encoding = encoding.replace("audio/wav", "audio/x-wav")
-    type = mimetypes.guess_type(encoding)[0]
-    if type == "audio/flac":  # flac is not supported by mimetypes
-        return "flac"
-    elif type is None:
-        return None
-    extension = mimetypes.guess_extension(type)
-    if extension is not None and extension.startswith("."):
-        extension = extension[1:]
-    return extension
-
-
-def encode_file_to_base64(f):
-    with open(f, "rb") as file:
-        encoded_string = base64.b64encode(file.read())
-        base64_str = str(encoded_string, "utf-8")
-        mimetype = get_mimetype(f)
-        return (
-            "data:"
-            + (mimetype if mimetype is not None else "")
-            + ";base64,"
-            + base64_str
-        )
-
-
-def encode_url_to_base64(url):
-    encoded_string = base64.b64encode(requests.get(url).content)
-    base64_str = str(encoded_string, "utf-8")
-    mimetype = get_mimetype(url)
-    return (
-        "data:" + (mimetype if mimetype is not None else "") + ";base64," + base64_str
-    )
-
-
-def encode_url_or_file_to_base64(path: str | Path):
-    path = str(path)
-    if is_valid_url(path):
-        return encode_url_to_base64(path)
-    else:
-        return encode_file_to_base64(path)
-
-
-def decode_base64_to_binary(encoding) -> Tuple[bytes, str | None]:
-    extension = get_extension(encoding)
-    try:
-        data = encoding.split(",")[1]
-    except IndexError:
-        data = ""
-    return base64.b64decode(data), extension
-
-
-def strip_invalid_filename_characters(filename: str, max_bytes: int = 200) -> str:
-    """Strips invalid characters from a filename and ensures that the file_length is less than `max_bytes` bytes."""
-    filename = "".join([char for char in filename if char.isalnum() or char in "._- "])
-    filename_len = len(filename.encode())
-    if filename_len > max_bytes:
-        while filename_len > max_bytes:
-            if len(filename) == 0:
-                break
-            filename = filename[:-1]
-            filename_len = len(filename.encode())
-    return filename
-
-
-def decode_base64_to_file(encoding, file_path=None, dir=None, prefix=None):
-    if dir is not None:
-        os.makedirs(dir, exist_ok=True)
-    data, extension = decode_base64_to_binary(encoding)
-    if file_path is not None and prefix is None:
-        filename = Path(file_path).name
-        prefix = filename
-        if "." in filename:
-            prefix = filename[0 : filename.index(".")]
-            extension = filename[filename.index(".") + 1 :]
-
-    if prefix is not None:
-        prefix = strip_invalid_filename_characters(prefix)
-
-    if extension is None:
-        file_obj = tempfile.NamedTemporaryFile(delete=False, prefix=prefix, dir=dir)
-    else:
-        file_obj = tempfile.NamedTemporaryFile(
-            delete=False,
-            prefix=prefix,
-            suffix="." + extension,
-            dir=dir,
-        )
-    file_obj.write(data)
-    file_obj.flush()
-    return file_obj
-
-
-def dict_or_str_to_json_file(jsn, dir=None):
-    if dir is not None:
-        os.makedirs(dir, exist_ok=True)
-
-    file_obj = tempfile.NamedTemporaryFile(
-        delete=False, suffix=".json", dir=dir, mode="w+"
-    )
-    if isinstance(jsn, str):
-        jsn = json.loads(jsn)
-    json.dump(jsn, file_obj)
-    file_obj.flush()
-    return file_obj
-
-
-def file_to_json(file_path: str | Path) -> Dict:
-    with open(file_path) as f:
-        return json.load(f)
-
-
-########################
-# Misc utils
-########################
-
-
-def synchronize_async(func: Callable, *args, **kwargs) -> Any:
-    """
-    Runs async functions in sync scopes. Can be used in any scope.
-
-    Example:
-        if inspect.iscoroutinefunction(block_fn.fn):
-            predictions = utils.synchronize_async(block_fn.fn, *processed_input)
-
-    Args:
-        func:
-        *args:
-        **kwargs:
-    """
-    return fsspec.asyn.sync(fsspec.asyn.get_loop(), func, *args, **kwargs)  # type: ignore
+from __future__ import annotations
+
+import asyncio
+import base64
+import json
+import mimetypes
+import os
+import pkgutil
+import shutil
+import tempfile
+from concurrent.futures import CancelledError
+from dataclasses import dataclass, field
+from datetime import datetime
+from enum import Enum
+from pathlib import Path
+from threading import Lock
+from typing import Any, Callable, Dict, List, Tuple
+
+import fsspec.asyn
+import httpx
+import huggingface_hub
+import requests
+from websockets.legacy.protocol import WebSocketCommonProtocol
+
+API_URL = "/api/predict/"
+WS_URL = "/queue/join"
+UPLOAD_URL = "/upload"
+RESET_URL = "/reset"
+SPACE_URL = "https://hf.space/{}"
+STATE_COMPONENT = "state"
+INVALID_RUNTIME = [
+    "NO_APP_FILE",
+    "CONFIG_ERROR",
+    "BUILD_ERROR",
+    "RUNTIME_ERROR",
+    "PAUSED",
+]
+BUILDING_RUNTIME = "BUILDING"
+
+__version__ = (pkgutil.get_data(__name__, "version.txt") or b"").decode("ascii").strip()
+
+
+class TooManyRequestsError(Exception):
+    """Raised when the API returns a 429 status code."""
+
+    pass
+
+
+class QueueError(Exception):
+    """Raised when the queue is full or there is an issue adding a job to the queue."""
+
+    pass
+
+
+class InvalidAPIEndpointError(Exception):
+    """Raised when the API endpoint is invalid."""
+
+    pass
+
+
+class Status(Enum):
+    """Status codes presented to client users."""
+
+    STARTING = "STARTING"
+    JOINING_QUEUE = "JOINING_QUEUE"
+    QUEUE_FULL = "QUEUE_FULL"
+    IN_QUEUE = "IN_QUEUE"
+    SENDING_DATA = "SENDING_DATA"
+    PROCESSING = "PROCESSSING"
+    ITERATING = "ITERATING"
+    FINISHED = "FINISHED"
+    CANCELLED = "CANCELLED"
+
+    @staticmethod
+    def ordering(status: "Status") -> int:
+        """Order of messages. Helpful for testing."""
+        order = [
+            Status.STARTING,
+            Status.JOINING_QUEUE,
+            Status.QUEUE_FULL,
+            Status.IN_QUEUE,
+            Status.SENDING_DATA,
+            Status.PROCESSING,
+            Status.ITERATING,
+            Status.FINISHED,
+            Status.CANCELLED,
+        ]
+        return order.index(status)
+
+    def __lt__(self, other: "Status"):
+        return self.ordering(self) < self.ordering(other)
+
+    @staticmethod
+    def msg_to_status(msg: str) -> "Status":
+        """Map the raw message from the backend to the status code presented to users."""
+        return {
+            "send_hash": Status.JOINING_QUEUE,
+            "queue_full": Status.QUEUE_FULL,
+            "estimation": Status.IN_QUEUE,
+            "send_data": Status.SENDING_DATA,
+            "process_starts": Status.PROCESSING,
+            "process_generating": Status.ITERATING,
+            "process_completed": Status.FINISHED,
+        }[msg]
+
+
+@dataclass
+class StatusUpdate:
+    """Update message sent from the worker thread to the Job on the main thread."""
+
+    code: Status
+    rank: int | None
+    queue_size: int | None
+    eta: float | None
+    success: bool | None
+    time: datetime | None
+
+
+def create_initial_status_update():
+    return StatusUpdate(
+        code=Status.STARTING,
+        rank=None,
+        queue_size=None,
+        eta=None,
+        success=None,
+        time=datetime.now(),
+    )
+
+
+@dataclass
+class JobStatus:
+    """The job status.
+
+    Keeps strack of the latest status update and intermediate outputs (not yet implements).
+    """
+
+    latest_status: StatusUpdate = field(default_factory=create_initial_status_update)
+    outputs: List[Any] = field(default_factory=list)
+
+
+@dataclass
+class Communicator:
+    """Helper class to help communicate between the worker thread and main thread."""
+
+    lock: Lock
+    job: JobStatus
+    deserialize: Callable[..., Tuple]
+    reset_url: str
+    should_cancel: bool = False
+
+
+########################
+# Network utils
+########################
+
+
+def is_valid_url(possible_url: str) -> bool:
+    headers = {"User-Agent": "gradio (https://gradio.app/; team@gradio.app)"}
+    try:
+        head_request = requests.head(possible_url, headers=headers)
+        if head_request.status_code == 405:
+            return requests.get(possible_url, headers=headers).ok
+        return head_request.ok
+    except Exception:
+        return False
+
+
+async def get_pred_from_ws(
+    websocket: WebSocketCommonProtocol,
+    data: str,
+    hash_data: str,
+    helper: Communicator | None = None,
+) -> Dict[str, Any]:
+    completed = False
+    resp = {}
+    while not completed:
+        # Receive message in the background so that we can
+        # cancel even while running a long pred
+        task = asyncio.create_task(websocket.recv())
+        while not task.done():
+            if helper:
+                with helper.lock:
+                    if helper.should_cancel:
+                        # Need to reset the iterator state since the client
+                        # will not reset the session
+                        async with httpx.AsyncClient() as http:
+                            reset = http.post(
+                                helper.reset_url, json=json.loads(hash_data)
+                            )
+                            # Retrieve cancel exception from task
+                            # otherwise will get nasty warning in console
+                            task.cancel()
+                            await asyncio.gather(task, reset, return_exceptions=True)
+                        raise CancelledError()
+            # Need to suspend this coroutine so that task actually runs
+            await asyncio.sleep(0.01)
+        msg = task.result()
+        resp = json.loads(msg)
+        if helper:
+            with helper.lock:
+                status_update = StatusUpdate(
+                    code=Status.msg_to_status(resp["msg"]),
+                    queue_size=resp.get("queue_size"),
+                    rank=resp.get("rank", None),
+                    success=resp.get("success"),
+                    time=datetime.now(),
+                    eta=resp.get("rank_eta"),
+                )
+                output = resp.get("output", {}).get("data", [])
+                if output and status_update.code != Status.FINISHED:
+                    try:
+                        result = helper.deserialize(*output)
+                    except Exception as e:
+                        result = [e]
+                    helper.job.outputs.append(result)
+                helper.job.latest_status = status_update
+        if resp["msg"] == "queue_full":
+            raise QueueError("Queue is full! Please try again.")
+        if resp["msg"] == "send_hash":
+            await websocket.send(hash_data)
+        elif resp["msg"] == "send_data":
+            await websocket.send(data)
+        completed = resp["msg"] == "process_completed"
+    return resp["output"]
+
+
+########################
+# Data processing utils
+########################
+
+
+def download_tmp_copy_of_file(
+    url_path: str, hf_token: str | None = None, dir: str | None = None
+) -> tempfile._TemporaryFileWrapper:
+    if dir is not None:
+        os.makedirs(dir, exist_ok=True)
+    headers = {"Authorization": "Bearer " + hf_token} if hf_token else {}
+    prefix = Path(url_path).stem
+    suffix = Path(url_path).suffix
+    file_obj = tempfile.NamedTemporaryFile(
+        delete=False,
+        prefix=prefix,
+        suffix=suffix,
+        dir=dir,
+    )
+    with requests.get(url_path, headers=headers, stream=True) as r:
+        with open(file_obj.name, "wb") as f:
+            shutil.copyfileobj(r.raw, f)
+    return file_obj
+
+
+def create_tmp_copy_of_file(
+    file_path: str, dir: str | None = None
+) -> tempfile._TemporaryFileWrapper:
+    if dir is not None:
+        os.makedirs(dir, exist_ok=True)
+    prefix = Path(file_path).stem
+    suffix = Path(file_path).suffix
+    file_obj = tempfile.NamedTemporaryFile(
+        delete=False,
+        prefix=prefix,
+        suffix=suffix,
+        dir=dir,
+    )
+    shutil.copy2(file_path, file_obj.name)
+    return file_obj
+
+
+def get_mimetype(filename: str) -> str | None:
+    if filename.endswith(".vtt"):
+        return "text/vtt"
+    mimetype = mimetypes.guess_type(filename)[0]
+    if mimetype is not None:
+        mimetype = mimetype.replace("x-wav", "wav").replace("x-flac", "flac")
+    return mimetype
+
+
+def get_extension(encoding: str) -> str | None:
+    encoding = encoding.replace("audio/wav", "audio/x-wav")
+    type = mimetypes.guess_type(encoding)[0]
+    if type == "audio/flac":  # flac is not supported by mimetypes
+        return "flac"
+    elif type is None:
+        return None
+    extension = mimetypes.guess_extension(type)
+    if extension is not None and extension.startswith("."):
+        extension = extension[1:]
+    return extension
+
+
+def encode_file_to_base64(f: str | Path):
+    with open(f, "rb") as file:
+        encoded_string = base64.b64encode(file.read())
+        base64_str = str(encoded_string, "utf-8")
+        mimetype = get_mimetype(str(f))
+        return (
+            "data:"
+            + (mimetype if mimetype is not None else "")
+            + ";base64,"
+            + base64_str
+        )
+
+
+def encode_url_to_base64(url: str):
+    encoded_string = base64.b64encode(requests.get(url).content)
+    base64_str = str(encoded_string, "utf-8")
+    mimetype = get_mimetype(url)
+    return (
+        "data:" + (mimetype if mimetype is not None else "") + ";base64," + base64_str
+    )
+
+
+def encode_url_or_file_to_base64(path: str | Path):
+    path = str(path)
+    if is_valid_url(path):
+        return encode_url_to_base64(path)
+    else:
+        return encode_file_to_base64(path)
+
+
+def decode_base64_to_binary(encoding) -> Tuple[bytes, str | None]:
+    extension = get_extension(encoding)
+    try:
+        data = encoding.split(",")[1]
+    except IndexError:
+        data = ""
+    return base64.b64decode(data), extension
+
+
+def strip_invalid_filename_characters(filename: str, max_bytes: int = 200) -> str:
+    """Strips invalid characters from a filename and ensures that the file_length is less than `max_bytes` bytes."""
+    filename = "".join([char for char in filename if char.isalnum() or char in "._- "])
+    filename_len = len(filename.encode())
+    if filename_len > max_bytes:
+        while filename_len > max_bytes:
+            if len(filename) == 0:
+                break
+            filename = filename[:-1]
+            filename_len = len(filename.encode())
+    return filename
+
+
+def decode_base64_to_file(encoding, file_path=None, dir=None, prefix=None):
+    if dir is not None:
+        os.makedirs(dir, exist_ok=True)
+    data, extension = decode_base64_to_binary(encoding)
+    if file_path is not None and prefix is None:
+        filename = Path(file_path).name
+        prefix = filename
+        if "." in filename:
+            prefix = filename[0 : filename.index(".")]
+            extension = filename[filename.index(".") + 1 :]
+
+    if prefix is not None:
+        prefix = strip_invalid_filename_characters(prefix)
+
+    if extension is None:
+        file_obj = tempfile.NamedTemporaryFile(delete=False, prefix=prefix, dir=dir)
+    else:
+        file_obj = tempfile.NamedTemporaryFile(
+            delete=False,
+            prefix=prefix,
+            suffix="." + extension,
+            dir=dir,
+        )
+    file_obj.write(data)
+    file_obj.flush()
+    return file_obj
+
+
+def dict_or_str_to_json_file(jsn, dir=None):
+    if dir is not None:
+        os.makedirs(dir, exist_ok=True)
+
+    file_obj = tempfile.NamedTemporaryFile(
+        delete=False, suffix=".json", dir=dir, mode="w+"
+    )
+    if isinstance(jsn, str):
+        jsn = json.loads(jsn)
+    json.dump(jsn, file_obj)
+    file_obj.flush()
+    return file_obj
+
+
+def file_to_json(file_path: str | Path) -> Dict:
+    with open(file_path) as f:
+        return json.load(f)
+
+
+###########################
+# HuggingFace Hub API Utils
+###########################
+def set_space_timeout(
+    space_id: str,
+    hf_token: str | None = None,
+    timeout_in_seconds: int = 300,
+):
+    headers = huggingface_hub.utils.build_hf_headers(
+        token=hf_token,
+        library_name="gradio_client",
+        library_version=__version__,
+    )
+    requests.post(
+        f"https://huggingface.co/api/spaces/{space_id}/sleeptime",
+        json={"seconds": timeout_in_seconds},
+        headers=headers,
+    )
+
+
+########################
+# Misc utils
+########################
+
+
+def synchronize_async(func: Callable, *args, **kwargs) -> Any:
+    """
+    Runs async functions in sync scopes. Can be used in any scope.
+
+    Example:
+        if inspect.iscoroutinefunction(block_fn.fn):
+            predictions = utils.synchronize_async(block_fn.fn, *processed_input)
+
+    Args:
+        func:
+        *args:
+        **kwargs:
+    """
+    return fsspec.asyn.sync(fsspec.asyn.get_loop(), func, *args, **kwargs)  # type: ignore
```

### Comparing `gradio_client-0.0.9/pyproject.toml` & `gradio_client-0.1.0/pyproject.toml`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-[build-system]
-requires = ["hatchling", "hatch-requirements-txt", "hatch-fancy-pypi-readme>=22.5.0"]
-build-backend = "hatchling.build"
-
-[project]
-name = "gradio_client"
-dynamic = ["version", "dependencies", "readme"]
-description = "Python library for easily interacting with trained machine learning models"
-license = "Apache-2.0"
-requires-python = ">=3.7"
-authors = [
-  { name = "Abubakar Abid", email = "team@gradio.app" },
-  { name = "Ali Abid", email = "team@gradio.app" },
-  { name = "Ali Abdalla", email = "team@gradio.app" },
-  { name = "Dawood Khan", email = "team@gradio.app" },
-  { name = "Ahsen Khaliq", email = "team@gradio.app" },
-  { name = "Pete Allen", email = "team@gradio.app" },
-  { name = "Freddy Boulton", email = "team@gradio.app" },
-]
-keywords = ["machine learning", "client", "API"]
-
-[project.urls]
-Homepage = "https://github.com/gradio-app/gradio"
-
-[tool.hatch.version]
-path = "gradio_client/version.txt"
-pattern = "(?P<version>.+)"
-
-[tool.hatch.metadata.hooks.requirements_txt]
-filename = "requirements.txt"
-
-[tool.hatch.metadata.hooks.fancy-pypi-readme]
-content-type = "text/markdown"
-fragments = [
-  { path = "README.md" },
-]
-
-[tool.hatch.build.targets.sdist]
-include = [
-  "/gradio_client",
-  "/README.md",
-  "/requirements.txt",
-]
-
-[tool.ruff]
-extend = "../../pyproject.toml"
-
-[tool.ruff.isort]
-known-first-party = [
-  "gradio_client"
-]
+[build-system]
+requires = ["hatchling", "hatch-requirements-txt", "hatch-fancy-pypi-readme>=22.5.0"]
+build-backend = "hatchling.build"
+
+[project]
+name = "gradio_client"
+dynamic = ["version", "dependencies", "readme"]
+description = "Python library for easily interacting with trained machine learning models"
+license = "Apache-2.0"
+requires-python = ">=3.7"
+authors = [
+  { name = "Abubakar Abid", email = "team@gradio.app" },
+  { name = "Ali Abid", email = "team@gradio.app" },
+  { name = "Ali Abdalla", email = "team@gradio.app" },
+  { name = "Dawood Khan", email = "team@gradio.app" },
+  { name = "Ahsen Khaliq", email = "team@gradio.app" },
+  { name = "Pete Allen", email = "team@gradio.app" },
+  { name = "Freddy Boulton", email = "team@gradio.app" },
+]
+keywords = ["machine learning", "client", "API"]
+
+[project.urls]
+Homepage = "https://github.com/gradio-app/gradio"
+
+[tool.hatch.version]
+path = "gradio_client/version.txt"
+pattern = "(?P<version>.+)"
+
+[tool.hatch.metadata.hooks.requirements_txt]
+filename = "requirements.txt"
+
+[tool.hatch.metadata.hooks.fancy-pypi-readme]
+content-type = "text/markdown"
+fragments = [
+  { path = "README.md" },
+]
+
+[tool.hatch.build.targets.sdist]
+include = [
+  "/gradio_client",
+  "/README.md",
+  "/requirements.txt",
+]
+
+[tool.ruff]
+extend = "../../pyproject.toml"
+
+[tool.ruff.isort]
+known-first-party = [
+  "gradio_client"
+]
```

### Comparing `gradio_client-0.0.9/PKG-INFO` & `gradio_client-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradio_client
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python library for easily interacting with trained machine learning models
 Project-URL: Homepage, https://github.com/gradio-app/gradio
 Author-email: Abubakar Abid <team@gradio.app>, Ali Abid <team@gradio.app>, Ali Abdalla <team@gradio.app>, Dawood Khan <team@gradio.app>, Ahsen Khaliq <team@gradio.app>, Pete Allen <team@gradio.app>, Freddy Boulton <team@gradio.app>
 License-Expression: Apache-2.0
 Keywords: API,client,machine learning
 Requires-Python: >=3.7
 Requires-Dist: fsspec
@@ -45,15 +45,15 @@
 
 Otherwise, the lightweight `gradio_client` package can be installed from pip (or pip3) and works with Python versions 3.9 or higher:
 
 ```bash
 $ pip install gradio_client
 ```
 
-## Usage
+## Basic Usage
 
 ### Connecting to a Space or a Gradio app
 
 Start by connecting instantiating a `Client` object and connecting it to a Gradio app that is running on Spaces (or anywhere else)!
 
 **Connecting to a Space**
 
@@ -67,28 +67,49 @@
 
 ```python
 from gradio_client import Client
 
 client = Client("abidlabs/my-private-space", hf_token="...") 
 ```
 
+**Duplicating a Space for private use**
+
+While you can use any public Space as an API, you may get rate limited by Hugging Face if you make too many requests. For unlimited usage of a Space, simply duplicate the Space to create a private Space,
+and then use it to make as many requests as you'd like!
+
+The `gradio_client` includes a class method: `Client.duplicate()` to make this process simple:
+
+```python
+from gradio_client import Client
+
+client = Client.duplicate("abidlabs/whisper") 
+client.predict("audio_sample.wav")  
+
+>> "This is a test of the whisper speech recognition model."
+```
+
+If you have previously duplicated a Space, re-running `duplicate()` will *not* create a new Space. Instead, the Client will attach to the previously-created Space. So it is safe to re-run the `Client.duplicate()` method multiple times. 
+
+**Note:** if the original Space uses GPUs, your private Space will as well, and your Hugging Face account will get billed based on the price of the GPU. To minimize charges, your Space will automatically go to sleep after 1 hour of inactivity. You can also set the hardware using the `hardware` parameter of `duplicate()`.
+
 
 **Connecting a general Gradio app**
 
 If your app is running somewhere else, just provide the full URL instead, including the "http://" or "https://". Here's an example of making predictions to a Gradio app that is running on a share URL:
 
 ```python
 from gradio_client import Client
 
 client = Client("https://bec81a83-5b5c-471e.gradio.live")
 ```
 
+
 ### Inspecting the API endpoints
 
-Once you have connected to a Gradio app, you can view the APIs that are available to you by calling the `Client.view_api()` method. For the Whisper Space, we see the following:
+Once you have connected to a Gradio app, you can view the APIs that are available to you by calling the `.view_api()` method. For the Whisper Space, we see the following:
 
 ```
 Client.predict() Usage Info
 ---------------------------
 Named API endpoints: 1
 
  - predict(input_audio, api_name="/predict") -> value_0
@@ -136,95 +157,10 @@
 client = Client("abidlabs/whisper")
 client.predict("https://audio-samples.github.io/samples/mp3/blizzard_unconditional/sample-0.mp3")
 
 >> "My thought I have nobody by a beauty and will as you poured. Mr. Rochester is serve in that so don't find simpus, and devoted abode, to at might in a r—"
 ```
 
 
-**Running jobs asyncronously**
-
-Oe should note that `.predict()` is a *blocking* operation as it waits for the operation to complete before returning the prediction. 
-
-In many cases, you may be better off letting the job run in the background until you need the results of the prediction. You can do this by creating a `Job` instance using the `.submit()` method, and then later calling `.result()` on the job to get the result. For example:
-
-```python
-from gradio_client import Client
-
-client = Client(space="abidlabs/en2fr")
-job = client.submit("Hello", api_name="/predict")  # This is not blocking
-
-# Do something else
-
-job.result()  # This is blocking
-
->> Bonjour
-```
-
-**Adding callbacks**
-
-Alternatively, one can add one or more callbacks to perform actions after the job has completed running, like this:
-
-```python
-from gradio_client import Client
-
-def print_result(x):
-    print("The translated result is: {x}")
-
-client = Client(space="abidlabs/en2fr")
-
-job = client.submit("Hello", api_name="/predict", result_callbacks=[print_result])
-
-# Do something else
-
->> The translated result is: Bonjour
-
-```
-
-**Status**
-
-The `Job` object also allows you to get the status of the running job by calling the `.status()` method. This returns a `StatusUpdate` object with the following attributes: `code` (the status code, one of a set of defined strings representing the status. See the `utils.Status` class), `rank` (the current position of this job in the queue), `queue_size` (the total queue size),  `eta` (estimated time this job will complete), `success` (a boolean representing whether the job completed successfully), and `time` (the time that the status was generated). 
-
-```py
-from gradio_client import Client
-
-client = Client(src="gradio/calculator")
-job = client.submit(5, "add", 4, api_name="/predict")
-job.status()
-
->> <Status.STARTING: 'STARTING'>
-```
-
-The `Job` object also has a `done()` instance method which returns a boolean indicating whether the job has completed.
-
-### Generator Endpoints
-
-Some Gradio API endpoints do not return a single value, rather they return a series of values. You can get the series of values that have been returned at any time from such a generator endpoint by running `job.outputs()`:
-
-```py
-from gradio_client import Client
-
-client = Client(src="gradio/count_generator")
-job = client.submit(3, api_name="/count")
-while not job.done():
-    time.sleep(0.1)
-job.outputs()
-
->> ['0', '1', '2']
-```
-
-Note that running `job.result()` on a generator endpoint only gives you the *first* value returned by the endpoint. 
-
-The `Job` object is also iterable, which means you can use it to display the results of a generator function as they are returned from the endpoint. Here's the equivalent example using the `Job` as a generator:
-
-```py
-from gradio_client import Client
-
-client = Client(src="gradio/count_generator")
-job = client.submit(3, api_name="/count")
-
-for o in job:
-    print(o)
+## Advanced Usage
 
->> 0
->> 1
->> 2
-```
+For more ways to use the Gradio Python Client, check out our dedicated Guide on the Python client, available here: https://www.gradio.app/getting-started-with-the-python-client/
```

