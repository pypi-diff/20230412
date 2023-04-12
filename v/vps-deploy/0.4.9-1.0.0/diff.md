# Comparing `tmp/vps-deploy-0.4.9.tar.gz` & `tmp/vps-deploy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vps-deploy-0.4.9.tar", last modified: Mon Sep 20 11:47:41 2021, max compression
+gzip compressed data, was "vps-deploy-1.0.0.tar", last modified: Wed Apr 12 00:07:46 2023, max compression
```

## Comparing `vps-deploy-0.4.9.tar` & `vps-deploy-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 ben       (1000) users      (998)        0 2021-09-20 11:47:41.937182 vps-deploy-0.4.9/
--rw-r--r--   0 ben       (1000) users      (998)     5491 2021-09-20 11:47:41.933182 vps-deploy-0.4.9/PKG-INFO
--rw-r--r--   0 ben       (1000) users      (998)     3842 2020-08-10 04:24:14.000000 vps-deploy-0.4.9/README.rst
--rw-r--r--   0 ben       (1000) users      (998)       38 2021-09-20 11:47:41.937182 vps-deploy-0.4.9/setup.cfg
--rw-r--r--   0 ben       (1000) users      (998)     3886 2021-09-20 11:45:28.000000 vps-deploy-0.4.9/setup.py
-drwxr-xr-x   0 ben       (1000) users      (998)        0 2021-09-20 11:47:41.933182 vps-deploy-0.4.9/vps_deploy/
--rw-r--r--   0 ben       (1000) users      (998)        0 2017-10-16 01:30:57.000000 vps-deploy-0.4.9/vps_deploy/__init__.py
--rw-r--r--   0 ben       (1000) users      (998)     8789 2020-07-14 05:14:10.000000 vps-deploy-0.4.9/vps_deploy/django_fabric.py
--rw-r--r--   0 ben       (1000) users      (998)    12106 2021-09-20 11:44:56.000000 vps-deploy-0.4.9/vps_deploy/django_fabric2.py
-drwxr-xr-x   0 ben       (1000) users      (998)        0 2021-09-20 11:47:41.933182 vps-deploy-0.4.9/vps_deploy.egg-info/
--rw-r--r--   0 ben       (1000) users      (998)     5491 2021-09-20 11:47:41.000000 vps-deploy-0.4.9/vps_deploy.egg-info/PKG-INFO
--rw-r--r--   0 ben       (1000) users      (998)      268 2021-09-20 11:47:41.000000 vps-deploy-0.4.9/vps_deploy.egg-info/SOURCES.txt
--rw-r--r--   0 ben       (1000) users      (998)        1 2021-09-20 11:47:41.000000 vps-deploy-0.4.9/vps_deploy.egg-info/dependency_links.txt
--rw-r--r--   0 ben       (1000) users      (998)       74 2021-09-20 11:47:41.000000 vps-deploy-0.4.9/vps_deploy.egg-info/requires.txt
--rw-r--r--   0 ben       (1000) users      (998)       11 2021-09-20 11:47:41.000000 vps-deploy-0.4.9/vps_deploy.egg-info/top_level.txt
+drwxr-xr-x   0 ben       (1000) users      (998)        0 2023-04-12 00:07:46.754970 vps-deploy-1.0.0/
+-rw-r--r--   0 ben       (1000) users      (998)    35061 2017-10-16 01:30:57.000000 vps-deploy-1.0.0/COPYING
+-rw-r--r--   0 ben       (1000) users      (998)     2985 2023-04-12 00:04:29.000000 vps-deploy-1.0.0/HISTORY.rst
+-rw-r--r--   0 ben       (1000) users      (998)     7370 2023-04-12 00:07:46.754970 vps-deploy-1.0.0/PKG-INFO
+-rw-r--r--   0 ben       (1000) users      (998)     3842 2020-08-10 04:24:14.000000 vps-deploy-1.0.0/README.rst
+-rw-r--r--   0 ben       (1000) users      (998)      103 2021-09-20 12:04:15.000000 vps-deploy-1.0.0/pyproject.toml
+-rw-r--r--   0 ben       (1000) users      (998)      697 2023-04-12 00:07:46.754970 vps-deploy-1.0.0/setup.cfg
+-rw-r--r--   0 ben       (1000) users      (998)       38 2021-09-20 12:04:37.000000 vps-deploy-1.0.0/setup.py
+drwxr-xr-x   0 ben       (1000) users      (998)        0 2023-04-12 00:07:46.754970 vps-deploy-1.0.0/vps_deploy/
+-rw-r--r--   0 ben       (1000) users      (998)        0 2017-10-16 01:30:57.000000 vps-deploy-1.0.0/vps_deploy/__init__.py
+-rw-r--r--   0 ben       (1000) users      (998)    12564 2023-03-08 23:51:43.000000 vps-deploy-1.0.0/vps_deploy/django_fabric2.py
+drwxr-xr-x   0 ben       (1000) users      (998)        0 2023-04-12 00:07:46.754970 vps-deploy-1.0.0/vps_deploy.egg-info/
+-rw-r--r--   0 ben       (1000) users      (998)     7370 2023-04-12 00:07:46.000000 vps-deploy-1.0.0/vps_deploy.egg-info/PKG-INFO
+-rw-r--r--   0 ben       (1000) users      (998)      285 2023-04-12 00:07:46.000000 vps-deploy-1.0.0/vps_deploy.egg-info/SOURCES.txt
+-rw-r--r--   0 ben       (1000) users      (998)        1 2023-04-12 00:07:46.000000 vps-deploy-1.0.0/vps_deploy.egg-info/dependency_links.txt
+-rw-r--r--   0 ben       (1000) users      (998)       74 2023-04-12 00:07:46.000000 vps-deploy-1.0.0/vps_deploy.egg-info/requires.txt
+-rw-r--r--   0 ben       (1000) users      (998)       11 2023-04-12 00:07:46.000000 vps-deploy-1.0.0/vps_deploy.egg-info/top_level.txt
```

### Comparing `vps-deploy-0.4.9/PKG-INFO` & `vps-deploy-1.0.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,143 +1,127 @@
-Metadata-Version: 1.1
-Name: vps-deploy
-Version: 0.4.9
-Summary: Common commands for deployment on a VPS.
-Home-page: https://gitlab.com/sturm/vps-deploy
-Author: Ben Sturmfels
-Author-email: ben@sturm.com.au
-License: GNU General Public License v3 or later (GPLv3+)
-Description: ==========
-        VPS Deploy
-        ==========
-        
-        This is a base set of Fabric deployment functions for projects based on Django,
-        Nginx, uWSGI Emperor, Memcached and PostgreSQL. Both Fabric 2 and legacy Fabric
-        1 systems are supported.
-        
-        Fabric is a handy tool for automating deployment processes. Unlike Salt or
-        Ansible, you're writing code from the beginning rather than diving into a Turing
-        Tarpit of templated YAML. Also unlike Salt, Ansible or shell scripts, Fabric
-        neatly coordinates both local and remote SSH tasks. While Fabric may not be your
-        best choice for provisioning, it works well as a simple and flexible tool for
-        automatic custom workflows.
-        
-        
-        Installation (Fabric 2.*)
-        -------------------------
-        
-        If Fabric 2 is available as an operating system package::
-        
-          $ sudo apt install fabric invoke
-          $ pip install --user vps-deploy
-        
-        Otherwise::
-        
-          $ pip install --user fabric invoke vps-deploy
-        
-        
-        Legacy installation for Fabric 1.*
-        ----------------------------------
-        
-        Fabric 1.* is recommended only for supporting existing projects. For new
-        projects, use Fabric 2.*.
-        
-        Since Fabric 1.* is Python 2-only and you're probably using a Python 3 virtual
-        env, you'll need to install Fabric and VPS Deploy as a `--user` package::
-        
-          # System package for Fabric, user package for vps-deploy:
-          $ sudo apt install fabric
-          $ pip install --user vps-deploy
-        
-          # All in user packages:
-          $ pip install --user fabric~=1.14 vps-deploy
-        
-        Alternately, while Fabric 1.* remains available for some operating systems, you
-        could also install it that way.
-        
-        
-        Getting started
-        ---------------
-        
-        To get started, create a `fabfile.py` in your top-level project directory. It
-        might look something like this:
-        
-        .. code:: python
-        
-           from fabric import task
-           from invoke.collection import Collection
-        
-           from vps_deploy import django_fabric2 as df2
-        
-           hosts = ['user@examplehost.com']
-        
-           @task(hosts=hosts)
-           def deploy(c):
-               df2.transfer_files_git(c)
-               df2.init(c)
-               df2.grep_for_pdb(c)
-               df2.lint(c)
-               df2.prepare_virtualenv(c)
-               df2.prepare_django(c)
-               df2.fix_permissions(c,
-                   # Sentry needs access to Git repo.
-                   read=[
-                       '.git', 'deploy', 'env', 'project'],
-                   read_write=['project', 'project/collected_static/CACHE'],
-               )
-               df2.reload_uwsgi(c)
-               df2.flush_memcached(c)
-               df2.update_nginx(c)
-        
-           ns = Collection(
-               deploy,
-               task(df2.download_postgres_db, hosts=hosts),
-               task(df2.mirror_postgres_db, hosts=hosts),
-               task(df2.mirror_media, hosts=hosts),
-           )
-           ns.configure({
-               # Built-in Fabric config.
-               'run': {
-                   'echo': True,
-                   # Needed so local commands work. Can also use FABRIC_RUN_REPLACE_ENV.
-                   'replace_env': False,
-                   # Needed for Guix. Can also use FABRIC_RUN_SHELL.
-                   # 'shell': '/run/current-system/profile/bin/bash',
-               },
-        
-               # Our custom project config.
-               'env': {
-                   'branch': 'master',
-                   'app_user': 'www-data',
-                   'db_name': 'exampledb',
-                   'project_dir': '/srv/exampleproject',
-                   'media_dir': 'project/media',
-                   'virtualenv': '/srv/venvs/exampleproject-django-py38',
-                   'site_name': 'examplesite',
-                   'requirements': 'requirements/production.txt',
-                   'settings': 'project.settings.live',
-                   'uwsgi_conf': 'deploy/uwsgi.ini',
-                   'nginx_conf': 'deploy/nginx.conf',
-                   'python': '/usr/bin/python3.8',
-               },
-           })
-        
-        
-        Deploying
-        ---------
-        
-        To make a deployment:
-        
-        `fab --prompt-for-sudo-password deploy`
-        
-        This depends on a few things being already set up, such as SSH access to the
-        server and having the server-site software and accounts set up. Those tend to to
-        be better handled with configuration management tools like Salt or Ansible (and
-        potentially triggered by Fabric!).
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
+==========
+VPS Deploy
+==========
+
+This is a base set of Fabric deployment functions for projects based on Django,
+Nginx, uWSGI Emperor, Memcached and PostgreSQL. Both Fabric 2 and legacy Fabric
+1 systems are supported.
+
+Fabric is a handy tool for automating deployment processes. Unlike Salt or
+Ansible, you're writing code from the beginning rather than diving into a Turing
+Tarpit of templated YAML. Also unlike Salt, Ansible or shell scripts, Fabric
+neatly coordinates both local and remote SSH tasks. While Fabric may not be your
+best choice for provisioning, it works well as a simple and flexible tool for
+automatic custom workflows.
+
+
+Installation (Fabric 2.*)
+-------------------------
+
+If Fabric 2 is available as an operating system package::
+
+  $ sudo apt install fabric invoke
+  $ pip install --user vps-deploy
+
+Otherwise::
+
+  $ pip install --user fabric invoke vps-deploy
+
+
+Legacy installation for Fabric 1.*
+----------------------------------
+
+Fabric 1.* is recommended only for supporting existing projects. For new
+projects, use Fabric 2.*.
+
+Since Fabric 1.* is Python 2-only and you're probably using a Python 3 virtual
+env, you'll need to install Fabric and VPS Deploy as a `--user` package::
+
+  # System package for Fabric, user package for vps-deploy:
+  $ sudo apt install fabric
+  $ pip install --user vps-deploy
+
+  # All in user packages:
+  $ pip install --user fabric~=1.14 vps-deploy
+
+Alternately, while Fabric 1.* remains available for some operating systems, you
+could also install it that way.
+
+
+Getting started
+---------------
+
+To get started, create a `fabfile.py` in your top-level project directory. It
+might look something like this:
+
+.. code:: python
+
+   from fabric import task
+   from invoke.collection import Collection
+
+   from vps_deploy import django_fabric2 as df2
+
+   hosts = ['user@examplehost.com']
+
+   @task(hosts=hosts)
+   def deploy(c):
+       df2.transfer_files_git(c)
+       df2.init(c)
+       df2.grep_for_pdb(c)
+       df2.lint(c)
+       df2.prepare_virtualenv(c)
+       df2.prepare_django(c)
+       df2.fix_permissions(c,
+           # Sentry needs access to Git repo.
+           read=[
+               '.git', 'deploy', 'env', 'project'],
+           read_write=['project', 'project/collected_static/CACHE'],
+       )
+       df2.reload_uwsgi(c)
+       df2.flush_memcached(c)
+       df2.update_nginx(c)
+
+   ns = Collection(
+       deploy,
+       task(df2.download_postgres_db, hosts=hosts),
+       task(df2.mirror_postgres_db, hosts=hosts),
+       task(df2.mirror_media, hosts=hosts),
+   )
+   ns.configure({
+       # Built-in Fabric config.
+       'run': {
+           'echo': True,
+           # Needed so local commands work. Can also use FABRIC_RUN_REPLACE_ENV.
+           'replace_env': False,
+           # Needed for Guix. Can also use FABRIC_RUN_SHELL.
+           # 'shell': '/run/current-system/profile/bin/bash',
+       },
+
+       # Our custom project config.
+       'env': {
+           'branch': 'master',
+           'app_user': 'www-data',
+           'db_name': 'exampledb',
+           'project_dir': '/srv/exampleproject',
+           'media_dir': 'project/media',
+           'virtualenv': '/srv/venvs/exampleproject-django-py38',
+           'site_name': 'examplesite',
+           'requirements': 'requirements/production.txt',
+           'settings': 'project.settings.live',
+           'uwsgi_conf': 'deploy/uwsgi.ini',
+           'nginx_conf': 'deploy/nginx.conf',
+           'python': '/usr/bin/python3.8',
+       },
+   })
+
+
+Deploying
+---------
+
+To make a deployment:
+
+`fab --prompt-for-sudo-password deploy`
+
+This depends on a few things being already set up, such as SSH access to the
+server and having the server-site software and accounts set up. Those tend to to
+be better handled with configuration management tools like Salt or Ansible (and
+potentially triggered by Fabric!).
```

### Comparing `vps-deploy-0.4.9/vps_deploy/django_fabric2.py` & `vps-deploy-1.0.0/vps_deploy/django_fabric2.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+# See my explainer of the problems with the built-in sudo():
+# https://github.com/fabric/fabric/issues/2091#issuecomment-871071304
+
 import datetime
 import io
 import sys
 import os
 
 import invoke
 from jinja2 import Template
@@ -34,15 +37,16 @@
         c.run('git config receive.denyCurrentBranch ignore')
 
     c.local("git push {c.user}@{c.host}:{env.project_dir} {env.branch}".format(
         env=c.env,
         c=c,
     ))
     with c.cd(c.env.project_dir):
-        c.run(f"git reset --hard {c.env.branch} --")
+        c.run(f'git checkout --force {c.env.branch}')
+        c.run(f'git reset --hard {c.env.branch} --')
 
 
 def transfer_files_git_pull(c):
     """A custom transfer_files_git that pulls rather than pushes changes.
 
     If the repository is private, you may need some sort of token. For GitLab,
     this would be a "deploy token" deploy token in the configuration of the
@@ -66,43 +70,45 @@
     if not exists(c, f'{c.env.project_dir}/env'):
         c.run(f'touch {c.env.project_dir}/env')
     media_dir = os.path.join(c.env.project_dir, c.env.media_dir)
     if not exists(c, media_dir):
         c.run(f'mkdir -p {media_dir}')
 
 
-def prepare_virtualenv(c):
+def prepare_virtualenv(c, pip_install_options=''):
     """Initialise a virtualenv and install required Python modules."""
 
     if not exists(c, c.env.virtualenv):
         c.sudo(f"mkdir -p $(dirname {c.env.virtualenv})")
         c.sudo(f'chown {c.user} $(dirname {c.env.virtualenv})')
 
         c.run("{env.python} -m venv --system-site-packages {env.virtualenv}".format(env=c.env))
     with c.cd(c.env.project_dir):
-        c.run("{env.virtualenv}/bin/python -m pip install -r {env.requirements}".format(
-            env=c.env))
+        c.run("{env.virtualenv}/bin/python -m pip install -r {env.requirements} {pip_install_options}".format(
+            env=c.env, pip_install_options=pip_install_options))
 
 
 def prepare_django(c, fail_level='WARNING'):
     # Clear all Python bytecode, just in case we've upgraded Python.
-    c.sudo(f'find {c.env.project_dir} -type d -name __pycache__ -exec rm -rf {{}} +') # Python 3
+    c.sudo(f'find {c.env.project_dir} -type d -name __pycache__ -exec rm -rf {{}} +')  # Python 3
 
     with c.cd(c.env.project_dir):
-        with c.prefix(f'source {c.env.project_dir}/env'):
+        # The `set -a` exports environment variables.
+        with c.prefix(f'set -a && source {c.env.project_dir}/env'):
             # Test configuration before we attempt to restart the application server.
             fail_level_arg = ''
             if fail_level:
                 fail_level_arg = f'--fail-level={fail_level}'
             c.run('{env.virtualenv}/bin/python manage.py check --deploy {fail_level_arg} --settings={env.settings}'.format(
-                env=c.env, fail_level_arg=fail_level_arg, user=c.env.app_user))
+                env=c.env, fail_level_arg=fail_level_arg))
 
             # Collect static files.
             c.run('{env.virtualenv}/bin/python manage.py collectstatic --settings={env.settings} -v0 --noinput --clear'.format(
-                env=c.env))
+                env=c.env,
+            ))
 
             # Migrate.
             #
             # Printing unicode characters during a migration can fail if remote
             # locale is something like "POSIX". Run `locale` to check.
             with c.prefix('LC_ALL=en_AU.utf8'):
                 c.run('{env.virtualenv}/bin/python manage.py migrate --settings={env.settings}'.format(
@@ -128,33 +134,37 @@
 
     for path in read:
         c.sudo(f'chmod --recursive g+rX {os.path.join(c.env.project_dir, path)}')
     for path in read_write:
         c.sudo(f'chmod --recursive g+rwX {os.path.join(c.env.project_dir, path)}')
 
 
-def _sudo_upload_template(c, local_path, remote_path, mode, owner=None, group=None):
+def sudo_upload_template(c, local_path, remote_path, mode, owner=None, group=None):
     # My hacked up replacement for upload template is permanently sudo and uses
     # full Jinja2 by default (both unlike Fabric 1).
     owner = c.user if owner is None else owner
     group = c.user if group is None else group
     with open(local_path) as f:
         content = f.read()
     t = Template(content)
-    output = t.render(env=c.env, **c.env) # Both env.X and just X.
+    output = t.render(env=c.env, **c.env)  # Both env.X and just X.
     m = io.StringIO(output)
     c.put(m, '/tmp/X')
     c.sudo(f'mv /tmp/X {remote_path}')
     c.sudo('chown {owner}:{group} {remote_path}'.format(
-        owner=owner, group=group, mode=mode, remote_path=remote_path))
+        owner=owner, group=group, remote_path=remote_path))
     c.sudo(f'chmod {mode} {remote_path}')
 
 
+# Backwards compatibility support for this now public function
+_sudo_upload_template = sudo_upload_template
+
+
 def reload_uwsgi(c):
-    _sudo_upload_template(
+    sudo_upload_template(
         c, c.env.uwsgi_conf, f'/etc/uwsgi-emperor/vassals/{c.env.site_name}.ini', '644')
 
     # Append secrets to uWSGI config on-the-fly.
     #
     # uWSGI config format for environment variables is different to a file
     # you might `source`. It has "env = " at the start instead of export,
     # doesn't mind whitespace in the values and treats quotes literally.
@@ -163,45 +173,45 @@
     # https://lists.gnu.org/archive/html/fab-user/2013-01/msg00005.html.
 
     # Don't use percent characters in environment variables because uWSGI will
     # silently drop them unless they are doubled-up (meaning that you'll have a
     # hard time tracking down the subtle bug).
     try:
         c.run(f"! grep '%' {c.env.project_dir}/env")
-    except invoke.exceptions.UnexpectedExit as e:
+    except invoke.exceptions.UnexpectedExit:
         print('Environment variables should not contain "%" due to its special use in uWSGI config.', file=sys.stderr)
         raise
 
     # Removes quotes as these are interpreted literally by uWSGI.
     c.sudo(f'echo "" >> /etc/uwsgi-emperor/vassals/{c.env.site_name}.ini')
-    c.sudo("""sed 's/export/env =/' {env.project_dir}/env | sed "s/['\\"]//g" >> /etc/uwsgi-emperor/vassals/{env.site_name}.ini""".format(env=c.env))
+    c.sudo("""sed 's/export//' {env.project_dir}/env | sed 's/^/env =/' | sed "s/['\\"]//g" >> /etc/uwsgi-emperor/vassals/{env.site_name}.ini""".format(env=c.env))
 
 
 def flush_memcached(c):
     """Clear cache by restarting the memcached server.
 
     By design, any user on the system can issue commands to memcached, including
     to flush the whole cache. Alternately, we could install libmemcached-tools
     and run `memcflush --servers localhost`.
 
     """
     c.run("echo flush_all | nc -w1 localhost 11211")
 
 
 def update_nginx(c):
-    _sudo_upload_template(
+    sudo_upload_template(
         c, c.env.nginx_conf, f'/etc/nginx/sites-available/{c.env.site_name}', '644')
     c.sudo("ln -s --force /etc/nginx/sites-available/{env.site_name} /etc/nginx/sites-enabled/{env.site_name}".format(
-            env=c.env))
+        env=c.env))
     c.sudo("/usr/sbin/nginx -t")
     c.sudo("/etc/init.d/nginx force-reload")
 
 
 def download_postgres_db(c):
-    tempfile = c.run('tempfile').stdout.strip()
+    tempfile = c.run('mktemp').stdout.strip()
     c.sudo('pg_dump --format=c {env.db_name} > {tempfile}'.format(
         env=c.env, tempfile=tempfile), user='postgres', pty=True)
     localtempfile = '{env.site_name}-{time:%Y-%m-%dT%H:%M:%S}.dump'.format(
         env=c.env, time=datetime.datetime.now())
     c.get(tempfile, localtempfile)
     # localtempfile = get(tempfile, local_path='%(basename)s')[0]
     c.sudo(f'rm -f {tempfile}')
@@ -254,15 +264,15 @@
     """
     if exclude is None:
         exclude = []
     elif isinstance(exclude, str):
         exclude = exclude.split(',')
     exclude += ['fabfile.py']
     exclusions = ' '.join([f"-path './{ex}' -prune -o" for ex in exclude])
-    c.local(f"! find {exclusions} -name '*.py' -exec grep -n '\\bpdb\\b' {{}} +")
+    c.local(f"! find {exclusions} -name '*.py' -exec grep -n '\\b\\(pdb\\|breakpoint\\)\\b' {{}} +")
 
 
 def django_test(c):
     c.local('python3 manage.py test --keepdb')
 
 
 def check_site_online(c):
@@ -284,37 +294,37 @@
         'cron.daily',
         'cron.weekly',
         'cron.monthly',
     }
     for job in periodic_jobs:
         basename = os.path.basename(job)
         if basename in typical_periodic_jobs:
-            _sudo_upload_template(
+            sudo_upload_template(
                 c,
                 job,
                 f'/etc/{basename}/{c.env.site_name}',
                 '755',
             )
         else:
             raise RuntimeError(f'Unexpected periodic job: {job}')
     for crontab in crontabs:
         name = os.path.basename(crontab).replace('cron.', '')
-        _sudo_upload_template(
+        sudo_upload_template(
             c,
             crontab,
             f'/etc/cron.d/{c.env.site_name}-{name}',
             '644',
             'root',
             'root',
         )
 
 
 def django_shell(c):
     with c.cd(c.env.project_dir):
-        c.run('source ./env && DJANGO_SETTINGS_MODULE={env.settings} {env.virtualenv}/bin/python manage.py shell'.format(env=c.env), pty=True)
+        c.run('set -a && source ./env && DJANGO_SETTINGS_MODULE={env.settings} {env.virtualenv}/bin/python manage.py shell'.format(env=c.env), pty=True)
 
 
 def bash(c):
     with c.cd(c.env.project_dir):
         c.run('bash', pty=True)
```

