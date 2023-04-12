# Comparing `tmp/miniircd-2.1.tar.gz` & `tmp/miniircd-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpbwgi4lhp/tmp2qfpq0n3/miniircd-2.1.tar", last modified: Mon Mar  8 19:34:39 2021, max compression
+gzip compressed data, was "miniircd-2.2.tar", last modified: Wed Apr 12 18:14:53 2023, max compression
```

## Comparing `miniircd-2.1.tar` & `miniircd-2.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2021-03-08 19:34:39.875242 miniircd-2.1/
--rw-rw-r--   0 joel      (1000) joel      (1000)     6585 2021-03-08 19:34:39.875242 miniircd-2.1/PKG-INFO
--rw-rw-r--   0 joel      (1000) joel      (1000)     4293 2021-03-08 19:20:20.000000 miniircd-2.1/README.md
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2021-03-08 19:34:39.875242 miniircd-2.1/miniircd.egg-info/
--rw-rw-r--   0 joel      (1000) joel      (1000)     6585 2021-03-08 19:34:39.000000 miniircd-2.1/miniircd.egg-info/PKG-INFO
--rw-rw-r--   0 joel      (1000) joel      (1000)      249 2021-03-08 19:34:39.000000 miniircd-2.1/miniircd.egg-info/SOURCES.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)        1 2021-03-08 19:34:39.000000 miniircd-2.1/miniircd.egg-info/dependency_links.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)       43 2021-03-08 19:34:39.000000 miniircd-2.1/miniircd.egg-info/entry_points.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)       51 2021-03-08 19:34:39.000000 miniircd-2.1/miniircd.egg-info/requires.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)        9 2021-03-08 19:34:39.000000 miniircd-2.1/miniircd.egg-info/top_level.txt
--rwxrwxr-x   0 joel      (1000) joel      (1000)    44168 2021-03-08 19:33:32.000000 miniircd-2.1/miniircd.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      150 2021-03-08 18:38:10.000000 miniircd-2.1/pyproject.toml
--rw-rw-r--   0 joel      (1000) joel      (1000)     1162 2021-03-08 19:34:39.875242 miniircd-2.1/setup.cfg
--rw-rw-r--   0 joel      (1000) joel      (1000)       38 2021-03-08 18:38:10.000000 miniircd-2.1/setup.py
+drwxrwxr-x   0 joel      (1000) docker     (997)        0 2023-04-12 18:14:53.176048 miniircd-2.2/
+-rw-rw-r--   0 joel      (1000) docker     (997)    18092 2021-07-14 19:00:39.000000 miniircd-2.2/LICENSE
+-rw-rw-r--   0 joel      (1000) docker     (997)     5494 2023-04-12 18:14:53.176048 miniircd-2.2/PKG-INFO
+-rw-rw-r--   0 joel      (1000) docker     (997)     4309 2021-04-05 19:00:01.000000 miniircd-2.2/README.md
+-rw-rw-r--   0 joel      (1000) docker     (997)       43 2021-03-08 18:38:10.000000 miniircd-2.2/entry_points.txt
+drwxrwxr-x   0 joel      (1000) docker     (997)        0 2023-04-12 18:14:53.176048 miniircd-2.2/miniircd.egg-info/
+-rw-rw-r--   0 joel      (1000) docker     (997)     5494 2023-04-12 18:14:53.000000 miniircd-2.2/miniircd.egg-info/PKG-INFO
+-rw-rw-r--   0 joel      (1000) docker     (997)      274 2023-04-12 18:14:53.000000 miniircd-2.2/miniircd.egg-info/SOURCES.txt
+-rw-rw-r--   0 joel      (1000) docker     (997)        1 2023-04-12 18:14:53.000000 miniircd-2.2/miniircd.egg-info/dependency_links.txt
+-rw-rw-r--   0 joel      (1000) docker     (997)       43 2023-04-12 18:14:53.000000 miniircd-2.2/miniircd.egg-info/entry_points.txt
+-rw-rw-r--   0 joel      (1000) docker     (997)       36 2023-04-12 18:14:53.000000 miniircd-2.2/miniircd.egg-info/requires.txt
+-rw-rw-r--   0 joel      (1000) docker     (997)        9 2023-04-12 18:14:53.000000 miniircd-2.2/miniircd.egg-info/top_level.txt
+-rwxrwxr-x   0 joel      (1000) docker     (997)    44412 2023-04-12 18:12:55.000000 miniircd-2.2/miniircd.py
+-rw-rw-r--   0 joel      (1000) docker     (997)      150 2021-03-08 18:38:10.000000 miniircd-2.2/pyproject.toml
+-rw-rw-r--   0 joel      (1000) docker     (997)     1226 2023-04-12 18:14:53.176048 miniircd-2.2/setup.cfg
+-rw-rw-r--   0 joel      (1000) docker     (997)       38 2021-03-08 18:38:10.000000 miniircd-2.2/setup.py
```

### Comparing `miniircd-2.1/README.md` & `miniircd-2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,19 +84,19 @@
 
 To create a new chroot jail for miniircd, edit the Makefile and change JAILDIR
 and JAILUSER to suit your needs, then run ``make jail`` as root. If you have a
 motd file or an SSL PEM file, you'll need to put them in the jail as well:
 
     cp miniircd.pem motd.txt /var/jail/miniircd
 
-Remember to specify the paths for `--state-dir`, `--log-dir`, `--motd` and
-`--ssl-pem-file` from within the jail, e.g.:
+Remember to specify the paths for `--state-dir`, `--channel-log-dir`, `--motd`
+and `--ssl-pem-file` from within the jail, e.g.:
 
-    miniircd --state-dir=/ --log-dir=/ --motd=/motd.txt --setuid=nobody \
-        --ssl-pem-file=/miniircd.pem --chroot=/var/jail/miniircd
+    miniircd --state-dir=/ --channel-log-dir=/ --motd=/motd.txt \
+        --setuid=nobody --ssl-pem-file=/miniircd.pem --chroot=/var/jail/miniircd
 
 Make sure your jail is writable by whatever user/group you are running the
 server as. Also, keep your jail clean. Ideally it should only contain the files
 mentioned above and the state/log files from miniircd. You should **not** place
 the miniircd script itself, or any executables, in the jail. In the end it
 should look something like this:
```

### Comparing `miniircd-2.1/miniircd.py` & `miniircd-2.2/miniircd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 #
-# Copyright (C) 2003-2021 Joel Rosdahl
+# Copyright (C) 2003-2023 Joel Rosdahl
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 2 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful, but
@@ -28,41 +28,37 @@
 import sys
 import tempfile
 import time
 
 from argparse import ArgumentParser, Namespace
 from datetime import datetime
 from logging.handlers import RotatingFileHandler
+from pathlib import Path
 from typing import Any, Collection, Dict, List, Optional, Sequence, Set
 
 Socket = socket.socket
 
-VERSION = "2.1"
-
-
-def create_directory(path: str) -> None:
-    if not os.path.isdir(path):
-        os.makedirs(path)
+VERSION = "2.2"
 
 
 class Channel:
     def __init__(self, server: "Server", name: bytes) -> None:
         self.server = server
         self.name = name
         self.members: Set["Client"] = set()
         self._topic = b""
         self._key: Optional[bytes] = None
-        self._state_path: Optional[str]
+        self._state_path: Optional[Path]
         if self.server.state_dir:
             fs_safe_name = (
                 name.decode(errors="ignore")
                 .replace("_", "__")
                 .replace("/", "_")
             )
-            self._state_path = f"{self.server.state_dir}/{fs_safe_name}"
+            self._state_path = self.server.state_dir / fs_safe_name
             self._read_state()
         else:
             self._state_path = None
 
     def add_member(self, client: "Client") -> None:
         self.members.add(client)
 
@@ -86,33 +82,31 @@
 
     def remove_client(self, client: "Client") -> None:
         self.members.discard(client)
         if not self.members:
             self.server.remove_channel(self)
 
     def _read_state(self) -> None:
-        if not (self._state_path and os.path.exists(self._state_path)):
+        if not (self._state_path and self._state_path.exists()):
             return
         data: Dict[str, Any] = {}
 
-        with open(self._state_path, "rb") as state_file:
-            exec(state_file.read(), {}, data)
-
+        exec(self._state_path.read_bytes(), {}, data)
         self._topic = data.get("topic", "")
         self._key = data.get("key")
 
     def _write_state(self) -> None:
         if not self._state_path:
             return
-        fd, path = tempfile.mkstemp(dir=os.path.dirname(self._state_path))
+        fd, path = tempfile.mkstemp(dir=self._state_path.parent)
         fp = os.fdopen(fd, "w")
         fp.write("topic = %r\n" % self.topic)
         fp.write("key = %r\n" % self.key)
         fp.close()
-        os.rename(path, self._state_path)
+        os.replace(path, self._state_path)
 
 
 class Client:
     __linesep_regexp = re.compile(rb"\r?\n")
     # The RFC limit for nicknames is 9 characters, but what the heck.
     __valid_nickname_regexp = re.compile(
         rb"^[][\`_^{|}A-Za-z][][\`_^{|}A-Za-z0-9-]{0,50}$"
@@ -129,18 +123,20 @@
         self.nickname = b""
         self.user = b""
         self.realname = b""
         if self.server.ipv6:
             host, port, _, _ = socket.getpeername()
         else:
             host, port = socket.getpeername()
+        assert isinstance(host, str)
+        assert isinstance(port, int)
         self.host = host.encode()
         self.port = port
         if self.server.cloak:
-            self.host = self.server.cloak
+            self.host = self.server.cloak.encode()
         self.__timestamp = time.time()
         self.__readbuffer = b""
         self.__writebuffer = b""
         self.__sent_ping = False
         if self.server.password:
             self.__handle_command = self.__pass_handler
         else:
@@ -191,19 +187,18 @@
     def __pass_handler(
         self, command: bytes, arguments: Sequence[bytes]
     ) -> None:
         server = self.server
         if command == b"PASS":
             if len(arguments) == 0:
                 self.reply_461(b"PASS")
+            elif arguments[0] == server.password.encode():
+                self.__handle_command = self.__registration_handler
             else:
-                if arguments[0] == server.password:
-                    self.__handle_command = self.__registration_handler
-                else:
-                    self.reply(b"464 :Password incorrect")
+                self.reply(b"464 :Password incorrect")
         elif command == b"QUIT":
             self.disconnect("Client quit")
 
     def __registration_handler(
         self, command: bytes, arguments: Sequence[bytes]
     ) -> None:
         server = self.server
@@ -324,15 +319,15 @@
             self.reply(b"303 %s :%s" % (self.nickname, b" ".join(online)))
 
         def join_handler() -> None:
             if len(arguments) < 1:
                 self.reply_461(b"JOIN")
                 return
             if arguments[0] == b"0":
-                for (channelname, channel) in self.channels.items():
+                for channelname, channel in self.channels.items():
                     self.message_channel(channel, b"PART", channelname, True)
                     self.channel_log(channel, b"left", meta=True)
                     server.remove_member_from_channel(self, channelname)
                 self.channels = {}
                 return
             self.__send_names(arguments, for_join=True)
 
@@ -551,15 +546,15 @@
                     self.message_channel(
                         channel,
                         b"TOPIC",
                         b"%s :%s" % (channelname, newtopic),
                         True,
                     )
                     self.channel_log(
-                        channel, b"set topic to %r" % newtopic, meta=True
+                        channel, b'set topic to "%s"' % newtopic, meta=True
                     )
                 else:
                     if channel.topic:
                         self.reply(
                             b"332 %s %s :%s"
                             % (self.nickname, channel.name, channel.topic)
                         )
@@ -670,15 +665,15 @@
         except KeyError:
             self.reply(
                 b"421 %s %s :Unknown command" % (self.nickname, command)
             )
 
     def socket_readable_notification(self) -> None:
         try:
-            data = self.socket.recv(2 ** 10)
+            data = self.socket.recv(2**10)
             if self.server.debug:
                 host = self.host.decode(errors="ignore")
                 self.server.print_debug(f"[{host}:{self.port}] -> {data!r}")
             quitmsg = "EOT"
         except socket.error as e:
             data = b""
             quitmsg = str(e)
@@ -743,16 +738,20 @@
         if meta:
             format_string = "[{}] * {} {}\n"
         else:
             format_string = "[{}] <{}> {}\n"
         timestamp = datetime.utcnow().strftime("%Y-%m-%d %H:%M:%S UTC")
         channel_name = irc_lower(channel.name).decode(errors="ignore")
         logname = channel_name.replace("_", "__").replace("/", "_")
-        logfile = f"{self.server.channel_log_dir}/{logname}.log"
-        logmsg = format_string.format(timestamp, self.nickname, message)
+        logfile = self.server.channel_log_dir / f"{logname}.log"
+        logmsg = format_string.format(
+            timestamp,
+            self.nickname.decode(errors="replace"),
+            message.decode(errors="replace"),
+        )
         with open(logfile, "a") as fp:
             fp.write(logmsg)
 
     def message_related(self, msg: bytes, include_self: bool = False) -> None:
         clients = set()
         if include_self:
             clients.add(self)
@@ -783,46 +782,53 @@
                 )
             self.reply(b"376 %s :End of /MOTD command" % self.nickname)
         else:
             self.reply(b"422 %s :MOTD File is missing" % self.nickname)
 
 
 class Server:
-    def __init__(self, args: Namespace) -> None:
-        self.ports = args.ports
-        self.password = args.password
-        self.ssl_cert_file = args.ssl_cert_file
-        self.ssl_key_file = args.ssl_key_file
-        self.motdfile = args.motd
-        self.verbose = args.verbose
-        self.ipv6 = args.ipv6
-        self.debug = args.debug
-        self.channel_log_dir = args.channel_log_dir
-        self.chroot = args.chroot
-        self.setuid = args.setuid
-        self.state_dir = args.state_dir
-        self.log_file = args.log_file
-        self.log_max_bytes = args.log_max_size * 1024 * 1024
-        self.log_count = args.log_count
+    def __init__(self, args: Namespace, ports: Collection[int]) -> None:
+        self.ports = ports
+        self.password: str = args.password
+        self.motdfile: Path = args.motd
+        self.verbose: bool = args.verbose
+        self.ipv6: bool = args.ipv6
+        self.debug: bool = args.debug
+        self.channel_log_dir: Path = args.channel_log_dir
+        self.chroot: Path = args.chroot
+        self.setuid: tuple[int, int] = args.setuid
+        self.state_dir: Path = args.state_dir
+        self.log_file: Path = args.log_file
+        self.log_max_bytes: int = args.log_max_size * 1024 * 1024
+        self.log_count: int = args.log_count
         self.logger: Optional[logging.Logger] = None
-        self.cloak = args.cloak
+        self.cloak: str = args.cloak
         self.name: bytes
+        self.ssl_context: "Optional[ssl.SSLContext]"
 
         if args.password_file:
-            with open(args.password_file, "r") as fp:
-                self.password = fp.read().strip("\n")
+            self.password = args.password_file.read_text().strip("\n")
+
+        if args.ssl_key_file:
+            import ssl
 
-        if self.ssl_key_file:
-            self.ssl = __import__("ssl")
+            ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
+            ssl_context.load_default_certs(purpose=ssl.Purpose.SERVER_AUTH)
+            ssl_context.load_cert_chain(
+                certfile=args.ssl_cert_file, keyfile=args.ssl_key_file
+            )
+            self.ssl_context = ssl_context
+        else:
+            self.ssl_context = None
 
         # Find key/cert files after daemonization if path is relative:
-        if self.ssl_cert_file and os.path.exists(self.ssl_cert_file):
-            self.ssl_cert_file = os.path.abspath(self.ssl_cert_file)
-        if self.ssl_key_file and os.path.exists(self.ssl_key_file):
-            self.ssl_key_file = os.path.abspath(self.ssl_key_file)
+        if args.ssl_cert_file and args.ssl_cert_file.exists():
+            args.ssl_cert_file = args.ssl_cert_file.resolve()
+        if args.ssl_key_file and args.ssl_key_file.exists():
+            args.ssl_key_file = args.ssl_key_file.resolve()
         # else: might exist in the chroot jail, so just continue
 
         if args.listen and self.ipv6:
             self.address = socket.getaddrinfo(
                 args.listen, None, proto=socket.IPPROTO_TCP
             )[0][4][0]
         elif args.listen:
@@ -832,32 +838,32 @@
         server_name_limit = 63  # From the RFC.
         self.name = socket.getfqdn(self.address)[:server_name_limit].encode()
 
         self.channels: Dict[bytes, Channel] = {}  # key: irc_lower(channelname)
         self.clients: Dict[Socket, Client] = {}
         self.nicknames: Dict[bytes, Client] = {}  # key: irc_lower(nickname)
         if self.channel_log_dir:
-            create_directory(self.channel_log_dir)
+            self.channel_log_dir.mkdir(parents=True, exist_ok=True)
         if self.state_dir:
-            create_directory(self.state_dir)
+            self.state_dir.mkdir(parents=True, exist_ok=True)
 
     def make_pid_file(self, filename: str) -> None:
         try:
             fd = os.open(filename, os.O_RDWR | os.O_CREAT | os.O_EXCL, 0o644)
             os.write(fd, b"%i\n" % os.getpid())
             os.close(fd)
         except Exception:
-            self.print_error("Could not create PID file %r" % filename)
+            self.print_error(f"Could not create PID file {filename!r}")
             sys.exit(1)
 
-    def remove_pid_file(self, filename: str) -> None:
+    def remove_pid_file(self, filename: Path) -> None:
         try:
-            os.remove(filename)
+            filename.unlink()
         except Exception:
-            self.print_error("Could not remove PID file %r" % filename)
+            self.print_error(f"Could not remove PID file {filename!r}")
 
     def daemonize(self) -> None:
         try:
             pid = os.fork()
             if pid > 0:
                 sys.exit(0)
         except OSError:
@@ -890,17 +896,17 @@
             channel = Channel(self, channelname)
             self.channels[irc_lower(channelname)] = channel
         return channel
 
     def get_motd_lines(self) -> Collection[str]:
         if self.motdfile:
             try:
-                return open(self.motdfile).readlines()
+                return self.motdfile.read_text().splitlines()
             except IOError:
-                return ["Could not read MOTD file %r." % self.motdfile]
+                return ["Could not read MOTD file {self.motdfile!r}."]
         else:
             return []
 
     def print_info(self, msg: str) -> None:
         if self.verbose:
             print(msg)
             sys.stdout.flush()
@@ -1015,48 +1021,43 @@
                 [],
                 10,
             )
             for x in iwtd:
                 if x in self.clients:
                     self.clients[x].socket_readable_notification()
                 else:
-                    conn, addr = x.accept()
-                    if self.ssl_key_file:
-                        try:
-                            conn = self.ssl.wrap_socket(
-                                conn,
-                                server_side=True,
-                                certfile=self.ssl_cert_file,
-                                keyfile=self.ssl_key_file,
-                            )
-                        except Exception as e:
-                            self.print_error(
-                                "SSL error for connection from"
-                                f" {addr[0]}:{addr[1]}: {e}"
-                            )
-                            continue
-                    try:
-                        self.clients[conn] = Client(self, conn)
-                        self.print_info(
-                            f"Accepted connection from {addr[0]}:{addr[1]}."
-                        )
-                    except socket.error:
-                        try:
-                            conn.close()
-                        except Exception:
-                            pass
+                    self._handle_server_socket(x)
             for x in owtd:
                 if x in self.clients:  # client may have been disconnected
                     self.clients[x].socket_writable_notification()
             now = time.time()
             if last_aliveness_check + 10 < now:
                 for client in list(self.clients.values()):
                     client.check_aliveness()
                 last_aliveness_check = now
 
+    def _handle_server_socket(self, server: Socket) -> None:
+        client, addr = server.accept()
+        if self.ssl_context:
+            try:
+                client = self.ssl_context.wrap_socket(client, server_side=True)
+            except Exception as e:
+                self.print_error(
+                    f"SSL error for connection from {addr[0]}:{addr[1]}: {e}"
+                )
+                return
+        try:
+            self.clients[client] = Client(self, client)
+            self.print_info(f"Accepted connection from {addr[0]}:{addr[1]}.")
+        except socket.error:
+            try:
+                client.close()
+            except Exception:
+                pass
+
 
 _ircstring_translation = bytes.maketrans(
     (string.ascii_lowercase.upper() + "[]\\^").encode(),
     (string.ascii_lowercase + "{}|~").encode(),
 )
 
 
@@ -1069,14 +1070,26 @@
         description="miniircd is a small and limited IRC server.",
     )
     ap.add_argument("--version", action="version", version=VERSION)
     ap.add_argument(
         "--channel-log-dir",
         metavar="X",
         help="store channel log in directory X",
+        type=Path,
+    )
+    if os.name == "posix":
+        ap.add_argument(
+            "--chroot",
+            metavar="X",
+            help="change filesystem root to directory X after startup"
+            " (requires root)",
+            type=Path,
+        )
+    ap.add_argument(
+        "--cloak", metavar="X", help="report X as the host for all clients"
     )
     ap.add_argument(
         "-d", "--daemon", action="store_true", help="fork and become a daemon"
     )
     ap.add_argument("--ipv6", action="store_true", help="use IPv6")
     ap.add_argument(
         "--debug", action="store_true", help="print debug messages to stdout"
@@ -1087,88 +1100,91 @@
     ap.add_argument(
         "--log-count",
         metavar="X",
         default=10,
         type=int,
         help="keep X log files; default: %(default)s",
     )
-    ap.add_argument("--log-file", metavar="X", help="store log in file X")
+    ap.add_argument(
+        "--log-file", metavar="X", help="store log in file X", type=Path
+    )
     ap.add_argument(
         "--log-max-size",
         metavar="X",
         default=10,
         type=int,
         help="set maximum log file size to X MiB; default: %(default)s MiB",
     )
     ap.add_argument(
-        "--motd", metavar="X", help="display file X as message of the day"
+        "--motd",
+        metavar="X",
+        help="display file X as message of the day",
+        type=Path,
+    )
+    ap.add_argument(
+        "--pid-file", metavar="X", help="write PID to file X", type=Path
     )
-    ap.add_argument("--pid-file", metavar="X", help="write PID to file X")
     ap.add_argument(
         "-p",
         "--password",
         metavar="X",
         help="require connection password X; default: no password",
     )
     ap.add_argument(
         "--password-file",
         metavar="X",
         help=(
             "require connection password stored in file X;"
             " default: no password"
         ),
+        type=Path,
     )
     ap.add_argument(
         "--ports",
         metavar="X",
         help="listen to ports X (a list separated by comma or whitespace);"
         " default: 6667 or 6697 if SSL is enabled",
     )
+    if os.name == "posix":
+        ap.add_argument(
+            "--setuid",
+            metavar="U[:G]",
+            help="change process user (and optionally group) after startup"
+            " (requires root)",
+        )
     ap.add_argument(
         "--ssl-cert-file",
         metavar="FILE",
         help="enable SSL with PEM certificate in FILE",
+        type=Path,
     )
     ap.add_argument(
         "--ssl-key-file",
         metavar="FILE",
         help="enable SSL with PEM key in FILE",
+        type=Path,
     )
     ap.add_argument(
         "-s",
         "--ssl-pem-file",
         metavar="FILE",
         help="enable SSL with key and certificate combined in FILE",
+        type=Path,
     )
     ap.add_argument(
         "--state-dir",
         metavar="X",
         help="save persistent channel state (topic, key) in directory X",
+        type=Path,
     )
     ap.add_argument(
         "--verbose",
         action="store_true",
         help="be verbose (print some progress messages to stdout)",
     )
-    ap.add_argument(
-        "--cloak", metavar="X", help="report X as the host for all clients"
-    )
-    if os.name == "posix":
-        ap.add_argument(
-            "--chroot",
-            metavar="X",
-            help="change filesystem root to directory X after startup"
-            " (requires root)",
-        )
-        ap.add_argument(
-            "--setuid",
-            metavar="U[:G]",
-            help="change process user (and optionally group) after startup"
-            " (requires root)",
-        )
 
     args = ap.parse_args()
 
     if bool(args.ssl_cert_file) != bool(args.ssl_key_file):
         args.error("Must specify both --ssl-cert-file and --ssl-key-file")
     if args.ssl_pem_file:
         if args.ssl_cert_file:
@@ -1226,18 +1242,18 @@
 
     ports = []
     for port in re.split(r"[,\s]+", args.ports):
         try:
             ports.append(int(port))
         except ValueError:
             ap.error("bad port: %r" % port)
-    args.ports = ports
-    server = Server(args)
+
+    server = Server(args, ports)
     if args.pid_file:
-        args.pid_file = os.path.abspath(args.pid_file)
+        args.pid_file = args.pid_file.resolve()
     if args.daemon:
         server.daemonize()
     if args.pid_file:
         server.make_pid_file(args.pid_file)
     try:
         server.start()
     except KeyboardInterrupt:
```

### Comparing `miniircd-2.1/setup.cfg` & `miniircd-2.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -19,27 +19,28 @@
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
 py_modules = miniircd
 entry_points = file: entry_points.txt
 
 [options.extras_require]
 dev = 
+	build
+	flake8
 	mypy
-	pyflakes
-	pycodestyle
 	nose
 	twine
-	pep517
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

