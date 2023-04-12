# Comparing `tmp/runjob-2.10.4-5-py2.py3-none-any.whl.zip` & `tmp/runjob-2.10.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 36633 bytes, number of entries: 22
--rw-r--r--  2.0 unx      174 b- defN 23-Apr-05 03:39 runjob/__init__.py
--rw-r--r--  2.0 unx       23 b- defN 23-Apr-01 13:33 runjob/_version.py
+Zip file size: 36681 bytes, number of entries: 22
+-rw-r--r--  2.0 unx      203 b- defN 23-Apr-09 07:12 runjob/__init__.py
+-rw-r--r--  2.0 unx       23 b- defN 23-Apr-12 07:37 runjob/_version.py
 -rw-r--r--  2.0 unx     2773 b- defN 23-Mar-29 12:34 runjob/bc_stat.py
 -rw-r--r--  2.0 unx     7141 b- defN 23-Mar-29 12:34 runjob/cluster.py
 -rw-r--r--  2.0 unx     5904 b- defN 23-Apr-05 06:38 runjob/config.py
 -rw-r--r--  2.0 unx     6702 b- defN 23-Mar-29 12:34 runjob/dag.py
 -rw-r--r--  2.0 unx    10857 b- defN 23-Mar-29 10:49 runjob/ins_type.json
--rw-r--r--  2.0 unx    17039 b- defN 23-Apr-06 10:41 runjob/job.py
--rw-r--r--  2.0 unx    14561 b- defN 23-Apr-03 10:22 runjob/jobstat.py
+-rw-r--r--  2.0 unx    17039 b- defN 23-Apr-11 10:52 runjob/job.py
+-rw-r--r--  2.0 unx    14636 b- defN 23-Apr-12 08:12 runjob/jobstat.py
 -rw-r--r--  2.0 unx     2687 b- defN 23-Apr-05 07:11 runjob/loger.py
--rw-r--r--  2.0 unx     4247 b- defN 23-Apr-06 10:28 runjob/qsub.py
+-rw-r--r--  2.0 unx     3223 b- defN 23-Apr-12 07:31 runjob/qsub.py
 -rw-r--r--  2.0 unx      248 b- defN 23-Mar-29 10:49 runjob/runjobconfig
 -rw-r--r--  2.0 unx     2044 b- defN 23-Mar-29 12:34 runjob/runtime.py
--rw-r--r--  2.0 unx     9134 b- defN 23-Apr-04 07:32 runjob/sge.py
--rw-r--r--  2.0 unx    24716 b- defN 23-Apr-06 10:53 runjob/sge_run.py
--rw-r--r--  2.0 unx    11598 b- defN 23-Apr-06 09:26 runjob/utils.py
--rw-r--r--  2.0 unx     1099 b- defN 23-Apr-07 06:54 runjob-2.10.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     2442 b- defN 23-Apr-07 06:54 runjob-2.10.4.dist-info/METADATA
--rw-r--r--  2.0 unx      119 b- defN 23-Apr-07 06:54 runjob-2.10.4.dist-info/WHEEL
--rw-r--r--  2.0 unx      186 b- defN 23-Apr-07 06:54 runjob-2.10.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-07 06:54 runjob-2.10.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1654 b- defN 23-Apr-07 06:54 runjob-2.10.4.dist-info/RECORD
-22 files, 125355 bytes uncompressed, 34023 bytes compressed:  72.9%
+-rw-r--r--  2.0 unx     9162 b- defN 23-Apr-09 03:54 runjob/sge.py
+-rw-r--r--  2.0 unx    25764 b- defN 23-Apr-12 08:13 runjob/sge_run.py
+-rw-r--r--  2.0 unx    12175 b- defN 23-Apr-12 08:12 runjob/utils.py
+-rw-r--r--  2.0 unx     1099 b- defN 23-Apr-12 09:00 runjob-2.10.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2442 b- defN 23-Apr-12 09:00 runjob-2.10.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-12 09:00 runjob-2.10.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx      217 b- defN 23-Apr-12 09:00 runjob-2.10.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-12 09:00 runjob-2.10.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1654 b- defN 23-Apr-12 09:00 runjob-2.10.5.dist-info/RECORD
+22 files, 126110 bytes uncompressed, 34071 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -42,26 +42,26 @@
 
 Filename: runjob/sge_run.py
 Comment: 
 
 Filename: runjob/utils.py
 Comment: 
 
-Filename: runjob-2.10.4.dist-info/LICENSE
+Filename: runjob-2.10.5.dist-info/LICENSE
 Comment: 
 
-Filename: runjob-2.10.4.dist-info/METADATA
+Filename: runjob-2.10.5.dist-info/METADATA
 Comment: 
 
-Filename: runjob-2.10.4.dist-info/WHEEL
+Filename: runjob-2.10.5.dist-info/WHEEL
 Comment: 
 
-Filename: runjob-2.10.4.dist-info/entry_points.txt
+Filename: runjob-2.10.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: runjob-2.10.4.dist-info/top_level.txt
+Filename: runjob-2.10.5.dist-info/top_level.txt
 Comment: 
 
-Filename: runjob-2.10.4.dist-info/RECORD
+Filename: runjob-2.10.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## runjob/__init__.py

```diff
@@ -1,5 +1,6 @@
 from .utils import JobQueue
 from .utils import Mylog as log
+from .loger import Formatter
 from ._version import __version__
 from .sge_run import RunSge as runsge
 from .config import load_config as Config
```

## runjob/_version.py

```diff
@@ -1 +1 @@
-__version__ = "2.10.4"
+__version__ = "2.10.5"
```

## runjob/jobstat.py

```diff
@@ -213,33 +213,33 @@
         print(style("-"*47, mode="bold"))
         # if len(success) + len(error) + running < submit:
         #    print style("{0} {1}".format("Warning:","some tasks may submite, but not running!" ), mode="bold", fore="red")
 
 
 def bcArgs():
     parser = argparse.ArgumentParser(
-        description="For query job status in batch compute.")
+        description="for query job status in batch compute.")
     parser.add_argument("-t", "--top", type=int, default=10,
-                        help="show top number job (default: 10)", metavar="<int>")
+                        help="show top number job. (default: 10)", metavar="<int>")
     parser.add_argument("-a", "--all", action="store_true", default=False,
-                        help="show all jobs")
+                        help="show all jobs.")
     parser.add_argument("-n", "--name", type=str,
-                        help="show jobName contains the specific name", metavar="<str>")
+                        help="show jobName contains the specific name.", metavar="<str>")
     parser.add_argument("-u", "--user", type=str, default=getpass.getuser(),
-                        help="show jobs with a user name matching, defualt: %s" % getpass.getuser(), metavar="<str>")
-    parser.add_argument("-r", '--regin', type=str, default="BEIJING", choices=['BEIJING', 'HANGZHOU', 'HUHEHAOTE', 'SHANGHAI',
-                        'ZHANGJIAKOU', 'CHENGDU', 'HONGKONG', 'QINGDAO', 'SHENZHEN'], help="batch compute regin, BEIJING by default")
+                        help="show jobs with a user name matching. (defualt: %s)" % getpass.getuser(), metavar="<str>")
+    parser.add_argument('-r', '--region', type=str, default="beijing", choices=['beijing', 'hangzhou', 'huhehaote', 'shanghai',
+                                                                               'zhangjiakou', 'chengdu', 'hongkong', 'qingdao', 'shenzhen'], help="batch compute region. (default: beijing)")
     parser.add_argument("-d", "--delete", type=str, nargs="*",
-                        help="delete job with jobId", metavar="<jobId>")
+                        help="delete job with jobId.", metavar="<jobId>")
     parser.add_argument("-j", "--job", type=str,
-                        help="description of the job", metavar="<jobId>")
+                        help="description of the job.", metavar="<jobId>")
     parser.add_argument('--access-key-id', type=str,
-                        help="AccessKeyID while access oss", metavar="<str>")
+                        help="AccessKeyID while access oss.", metavar="<str>")
     parser.add_argument('--access-key-secret', type=str,
-                        help="AccessKeySecret while access oss", metavar="<str>")
+                        help="AccessKeySecret while access oss.", metavar="<str>")
     parser.add_argument('-ini', '--ini',
                         help="input configfile for configurations search.", metavar="<configfile>")
     parser.add_argument("-config", '--config',   action='store_true',
                         help="show configurations and exit.",  default=False)
     # parser.add_argument("-l", "--logdir", type=str,
     # help="summary job status in you job directory", metavar="<jobfile>")
     parser.add_argument('-v', '--version',
@@ -253,15 +253,15 @@
     conf = load_config()
     if args.ini:
         conf.update_config(args.ini)
     conf.update_dict(**args.__dict__)
     if args.config:
         print_config(conf)
         sys.exit()
-    region = REGION.get(args.regin, CN_BEIJING)
+    region = REGION.get(args.region.upper(), CN_BEIJING)
     access_key_id = conf.get("args", "access_key_id")
     access_key_secret = conf.get("args", "access_key_secret")
     if access_key_id is None:
         access_key_id = conf.get("OSS", "access_key_id")
     if access_key_secret is None:
         access_key_secret = conf.get("OSS", "access_key_secret")
     if access_key_secret is None or access_key_id is None:
```

## runjob/qsub.py

```diff
@@ -4,49 +4,14 @@
 from . import dag
 from .utils import *
 from .job import Jobfile
 from .sge_run import RunSge
 from .config import load_config
 
 
-class CleanUpSingal(Thread):
-
-    def __init__(self, obj=None):
-        super(CleanUpSingal, self).__init__()
-        signal.signal(signal.SIGINT, self.signal_handler)
-        signal.signal(signal.SIGTERM, self.signal_handler)
-        signal.signal(signal.SIGUSR1, self.signal_handler)
-        self.obj = obj
-        self.mode = obj.mode
-        self.daemon = True
-        self.killed = False
-
-    def run(self):
-        time.sleep(1)
-
-    def clean(self):
-        if self.mode == "sge":
-            self.obj.qdel(name=self.obj.name)
-            for jb in self.obj.jobqueue.queue:
-                jb.remove_all_stat_files()
-                self.obj.log_kill(jb)
-        for j, p in self.obj.localprocess.items():
-            if p.poll() is None:
-                terminate_process(p.pid)
-            p.wait()
-            self.obj.log_kill(self.obj.totaljobdict[j])
-
-    def signal_handler(self, signum, frame):
-        if not self.killed:
-            self.clean()
-            self.obj.sumstatus()
-            self.killed = True
-        sys.exit(signum)
-
-
 class qsub(RunSge):
 
     def __init__(self, config=None):
 
         self.conf = config
         self.jobfile = config.jobfile
         self.queue = config.queue
@@ -63,25 +28,28 @@
         self.totaljobdict = {jf.name: jf for jf in jf.totaljobs}
         self.orders = jf.orders()
         self.is_run = False
         self.localprocess = {}
         self.cloudjob = {}
         self.jobsgraph = dag.DAG()
         self.has_success = []
-        self.create_graph()
+        self.__create_graph()
         self.logger.info("Total jobs to submit: %s" %
                          ", ".join([j.name for j in self.jobs]))
         self.logger.info("All logs can be found in %s directory", self.logdir)
         self.check_already_success()
         self.maxjob = self.maxjob or len(self.jobs)
         self.jobqueue = JobQueue(maxsize=min(max(self.maxjob, 1), 1000))
-        self.rate = Fraction(config.rate or 3).limit_denominator()
+        self.check_rate = Fraction(
+            config.max_check or 3).limit_denominator()
+        self.sub_rate = Fraction(
+            config.max_submit or 30).limit_denominator()
         self.sge_jobid = {}
 
-    def create_graph(self):
+    def __create_graph(self):
         for k, v in self.orders.items():
             self.jobsgraph.add_node_if_not_exists(k)
             for i in v:
                 self.jobsgraph.add_node_if_not_exists(i)
                 self.jobsgraph.add_edge(i, k)
         for jn in self.jobsgraph.all_nodes.copy():
             if jn not in self.jobnames:
@@ -90,19 +58,15 @@
             names = [i for i, j in Counter(
                 self.jf.alljobnames).items() if j > 1]
             self.throw("duplicate job name: %s" % " ".join(names))
         if self.jobsgraph.size() == 0:
             for jb in self.jobs:
                 self.jobsgraph.add_node_if_not_exists(jb.name)
 
-    def clean_resource(self):
-        h = CleanUpSingal(obj=self)
-        h.start()
-
-    def qdel(self, name="", jobname=""):
+    def _qdel(self, name="", jobname=""):
         if name:
             call_cmd(['qdel', "*_%d" % os.getpid()])
             self.sge_jobid.clear()
         if jobname:
             jobid = self.sge_jobid.get(jobname, jobname)
             call_cmd(["qdel", jobid])
             if jobname in self.sge_jobid:
@@ -116,12 +80,12 @@
     if args.jobfile is None:
         parser.error("the following arguments are required: -j/--jobfile")
     if args.local:
         args.mode = "local"
     conf.update_dict(**args.__dict__)
     logger = Mylog(logfile=args.log, level=args.debug and "debug" or "info")
     qjobs = qsub(config=conf)
-    qjobs.run(times=args.resub, resubivs=args.resubivs)
+    qjobs.run(retry=args.resub, ivs=args.resubivs)
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

## runjob/sge.py

```diff
@@ -20,36 +20,36 @@
 
 class ParseSingal(Thread):
 
     def __init__(self, obj=None, name="", mode="sge", conf=None):
         super(ParseSingal, self).__init__()
         signal.signal(signal.SIGINT, self.signal_handler)
         signal.signal(signal.SIGTERM, self.signal_handler)
-        signal.signal(signal.SIGUSR1, self.signal_handler_ui)
+        signal.signal(signal.SIGUSR1, self.signal_handler_us)
         self.obj = obj
         self.name = name
         self.mode = mode
         self.conf = conf
         self.daemon = True
         self.killed = False
 
     def run(self):
         time.sleep(1)
 
     def clean_jobs(self):
         self.obj.clean_jobs()
 
     def signal_handler(self, signum, frame):
-        if not self.killed:
+        if not self.killed and not self.obj.is_success:
             self.clean_jobs()
             self.obj.sumstatus()
             self.killed = True
         os._exit(signum)  # force exit
 
-    def signal_handler_ui(self, signum, frame):
+    def signal_handler_us(self, signum, frame):
         if not self.killed:
             self.clean_jobs()
             self.obj.sumstatus()
             self.killed = True
         sys.exit(signum)  # SystemExit Exception
```

## runjob/sge_run.py

```diff
@@ -20,15 +20,14 @@
 
 
 class RunSge(object):
 
     def __init__(self, config=None):
         '''
         all attribute of config:
-
             @jobfile <file, list>: required
             @jobname <str>: default: basename(jobfile)
             @mode <str>: default: sge
             @queue <list>: default: all access queue
             @num <int>: default: total jobs
             @startline <int>: default: 1
             @endline <int>: default: None
@@ -62,44 +61,49 @@
         self.name = self.sgefile.name
         self.totaljobdict = {j.jobname: j for j in self.jobs}
         self.is_run = False
         self.localprocess = {}
         self.cloudjob = {}
         self.jobsgraph = dag.DAG()
         self.has_success = []
-        self.depency_jobs()
-        self.group_jobs()
+        self.__add_depency_for_wait()
+        self.__group_jobs()
         self.init_callback()
+        if config.loglevel is not None:
+            self.logger.setLevel(config.loglevel)
         self.logger.info("Total jobs to submit: %s" %
                          ", ".join([j.name for j in self.jobs]))
         self.logger.info("All logs can be found in %s directory", self.logdir)
         self.check_already_success()
         self.maxjob = self.maxjob or len(self.jobs)
         self.jobqueue = JobQueue(maxsize=min(max(self.maxjob, 1), 1000))
         self.conf.jobqueue = self.jobqueue
         self.conf.logger = self.logger
         self.conf.cloudjob = self.cloudjob
-        self.rate = Fraction(config.rate or 3).limit_denominator()
+        self.check_rate = Fraction(
+            config.max_check or 3).limit_denominator()
+        self.sub_rate = Fraction(
+            config.max_submit or 30).limit_denominator()
         self.sge_jobid = {}
 
-    def depency_jobs(self):
+    def __add_depency_for_wait(self):
         cur_jobs, dep_jobs = [], []
         for j in self.jobs[:]:
             if j.rawstring == "wait":
                 if cur_jobs:
                     dep_jobs = cur_jobs[:]
                     cur_jobs = []
             else:
                 self.jobsgraph.add_node_if_not_exists(j.jobname)
                 if dep_jobs:
                     for dep_j in dep_jobs:
                         self.jobsgraph.add_edge(dep_j.jobname, j.jobname)
                 cur_jobs.append(j)
 
-    def group_jobs(self):
+    def __group_jobs(self):
         jobs_groups = []
         jgs = []
         for j in self.jobs[:]:
             if j.rawstring == "wait":
                 self.jobs.remove(j)
                 if jgs:
                     jobs_groups.append(jgs)
@@ -109,28 +113,28 @@
         if jgs:
             jobs_groups.append(jgs)
         for wait_groups in jobs_groups:
             i = 0
             for n, jb in enumerate(wait_groups):
                 if jb.groups:
                     if n >= i:
-                        self._make_groups(wait_groups[n:n+jb.groups])
+                        self.__make_groups(wait_groups[n:n+jb.groups])
                         i = jb.groups+n
                     else:
                         self.throw('groups conflict in "%s" line number %d: "%s"' % (self.jfile,
                                                                                      jb.linenum, jb.cmd0))
                 elif n >= i and (n-i) % self.groups == 0:
                     gs = []
                     for j in wait_groups[n:n+self.groups]:
                         if j.groups:
                             break
                         gs.append(j)
-                    self._make_groups(gs)
+                    self.__make_groups(gs)
 
-    def _make_groups(self, jobs=None):
+    def __make_groups(self, jobs=None):
         if len(jobs) > 1:
             j_header = jobs[0]
             for j in jobs[1:]:
                 j_header.rawstring += "\n" + j.rawstring
                 if j in self.jobs:
                     self.jobs.remove(j)
                 self.jobsgraph.delete_node_if_exists(j.jobname)
@@ -192,15 +196,16 @@
             name = self.cloudjob[name]
         if job.is_fail:
             level = "error"
         elif job.status == "resubmit":
             level = "warn"
         else:
             level = "info"
-        getattr(self.logger, level)("job %s status %s", name, job.status)
+        if not job.is_wait:
+            getattr(self.logger, level)("job %s status %s", name, job.status)
 
     def log_kill(self, jb):
         '''
         may be status delay
         '''
         if not jb.is_killed:
             jb.set_kill()
@@ -284,23 +289,25 @@
             self.log_status(job)
             if job.host == "batchcompute":
                 with open(logfile, "a") as fo:
                     fo.write("[%s] %s\n" % (
                         datetime.today().strftime("%F %X"), job.status.upper()))
         return status
 
-    def set_rate(self, rate=3):
-        if rate:
-            self.rate = Fraction(rate).limit_denominator()
+    def set_rate(self, check_rate=0, sub_rate=0):
+        if check_rate:
+            self.check_rate = Fraction(check_rate).limit_denominator()
+        if sub_rate:
+            self.sub_rate = Fraction(sub_rate).limit_denominator()
 
     def jobcheck(self):
         if self.mode == "batchcompute":
-            self.set_rate(1)
+            self.set_rate(check_rate=1)
         rate_limiter = RateLimiter(
-            max_calls=self.rate.numerator, period=self.rate.denominator)
+            max_calls=self.check_rate.numerator, period=self.check_rate.denominator)
         while True:
             for jb in self.jobqueue.queue:
                 with rate_limiter:
                     try:
                         js = self.jobstatus(jb)
                     except:
                         self.logger.error(
@@ -326,14 +333,18 @@
                         self.deletejob(jb)
                         self.jobqueue.get(jb)
                         self.jobsgraph.delete_node_if_exists(jb.jobname)
                         if self.strict:
                             self.throw("Error job: %s, exit" % jb.jobname)
 
     def qdel(self, name="", jobname=""):
+        self._qdel(name=name, jobname=jobname)
+
+    # Override these methods to implement other subclass
+    def _qdel(self, name="", jobname=""):
         if name:
             call_cmd(['qdel', "%s_%d*" % (name, os.getpid())])
             self.sge_jobid.clear()
         if jobname:
             jobid = self.sge_jobid.get(jobname, jobname)
             call_cmd(["qdel", jobid])
             if jobname in self.sge_jobid:
@@ -380,15 +391,15 @@
             if job.host is not None and job.host in ["localhost", "local"]:
                 cmd = "echo 'Your job (\"%s\") has been submitted in localhost' && " % job.name + job.cmd
                 if job.subtimes > 0:
                     cmd = cmd.replace("RUNNING", "RUNNING (re-submit)")
                     time.sleep(self.resubivs)
                 if job.workdir != self.workdir:
                     if not os.path.isdir(job.workdir):
-                        os.makedirs(job.workdir)
+                        mkdir(job.workdir)
                     os.chdir(job.workdir)
                     p = Popen(cmd, shell=True, stdout=logcmd,
                               stderr=logcmd, env=os.environ)
                     os.chdir(self.workdir)
                 else:
                     p = Popen(cmd, shell=True, stdout=logcmd,
                               stderr=logcmd, env=os.environ)
@@ -432,56 +443,72 @@
         match = QSUB_JOB_ID_DECODER.search(output.decode())
         if match:
             jobid = match.group(1)
         else:
             self.throw(output.decode())
         return jobid, output.decode()
 
-    def run(self, sec=2, times=0, resubivs=2):
+    def run(self, retry=0, ivs=2, sec=2):
         '''
+        @retry: retry times, default: 0
+        @ivs: retry ivs sec, default: 2
         @sec: submit epoch ivs, default: 2
-        @times: resubmit times, default: 0
-        @resubivs: resubmit ivs sec, default: 2
         '''
         self.is_run = True
-        self.times = max(0, times)
-        self.resubivs = max(resubivs, 0)
+        self.times = max(0, retry)
+        self.resubivs = max(ivs, 0)
         for jn in self.has_success:
             self.logger.info("job %s status already success", jn)
         if len(self.jobsgraph.graph) == 0:
             return
         self.clean_resource()
         p = Thread(target=self.jobcheck)
         p.setDaemon(True)
         p.start()
+        mkdir(self.logdir)
+        mkdir(self.workdir)
+        max_calls = 10000
         if self.mode == "batchcompute":
             access_key_id = self.conf.args.access_key_id or self.conf.access_key_id
             access_key_secret = self.conf.args.access_key_secret or self.conf.access_key_secret
-            region = REGION.get(self.conf.args.region, CN_BEIJING)
+            region = REGION.get(self.conf.args.region.upper(), CN_BEIJING)
             client = Client(region, access_key_id, access_key_secret)
             quotas = client.get_quotas().AvailableClusterInstanceType
             cfg_path = os.path.join(os.path.dirname(__file__), "ins_type.json")
             with open(cfg_path) as fi:
                 self.conf.it_conf = json.load(fi)
             availableTypes = [i for i in quotas if i in self.conf.it_conf]
             self.conf.availableTypes = sorted(availableTypes, key=lambda x: (
                 self.conf.it_conf[x]["cpu"], self.conf.it_conf[x]["memory"]))
             self.conf.client = self.client = client
+            max_calls = self.sub_rate.numerator
+        elif self.mode == "sge":
+            max_calls = self.sub_rate.numerator
+        sub_rate_limiter = RateLimiter(
+            max_calls=max_calls, period=self.sub_rate.denominator)
         while True:
             subjobs = self.jobsgraph.ind_nodes()
             if len(subjobs) == 0:
                 break
-            for j in sorted(subjobs):
-                jb = self.totaljobdict[j]
-                if jb in self.jobqueue._queue:
-                    continue
-                self.submit(jb)
+            for jb in self.pending_jobs(*subjobs):
+                with sub_rate_limiter:
+                    self.submit(jb)
             time.sleep(sec)
         if not self.is_success:
             os.kill(os.getpid(), signal.SIGUSR1)
+        else:
+            self.sumstatus()
+
+    def pending_jobs(self, *names):
+        jobs = []
+        for j in sorted(names):
+            jb = self.totaljobdict[j]
+            if jb not in self.jobqueue:
+                jobs.append(jb)
+        return jobs
 
     @property
     def logger(self):
         return logging.getLogger(__name__)
 
     def clean_jobs(self):
         if self.mode == "sge":
@@ -602,12 +629,12 @@
     if args.logdir is None:
         args.logdir = "runjob_"+os.path.basename(args.jobfile) + "_log_dir"
     args.logdir = os.path.join(args.workdir, args.logdir)
     conf.update_dict(**args.__dict__)
     logger = Mylog(logfile=args.log,
                    level="debug" if args.debug else "info", name=__name__)
     runsge = RunSge(config=conf)
-    runsge.run(times=args.resub, resubivs=args.resubivs)
+    runsge.run(retry=args.resub, ivs=args.resubivs)
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

## runjob/utils.py

```diff
@@ -63,14 +63,17 @@
             if name in self._queue:
                 self._queue.remove(name)
                 return name
             else:
                 raise KeyError(name)
         return self._queue.pop()
 
+    def __contains__(self, item):
+        return item in self._queue
+
     def __str__(self):
         return self._queue.__str__()
 
     __repr__ = __str__
 
     @property
     def length(self):
@@ -155,14 +158,22 @@
 
 def now():
     if hasattr(time, 'monotonic'):
         return time.monotonic()
     return time.time()
 
 
+def mkdir(path):
+    if not os.path.isdir(path):
+        try:
+            os.makedirs(path)
+        except:
+            pass
+
+
 def terminate_process(pid):
     try:
         pproc = psutil.Process(pid)
         for cproc in pproc.children(recursive=True):
             # cproc.terminate() # SIGTERM
             cproc.kill()  # SIGKILL
         # pproc.terminate()
@@ -196,90 +207,92 @@
             return False
     return False
 
 
 def common_parser():
     p = argparse.ArgumentParser(add_help=False)
     common = p.add_argument_group("common arguments")
+    common.add_argument('-v', '--version',
+                        action='version', version="v" + __version__)
     common.add_argument("-j", "--jobfile", type=str,
-                        help="the input jobfile, " + style("required", fore="green", mode="bold"), metavar="<jobfile>")
+                        help="the input jobfile. " + style("(required)", fore="green", mode="bold"), metavar="<jobfile>")
     common.add_argument("-n", "--num", type=int,
-                        help="the max job number runing at the same time. default: all in your job file, max 1000", metavar="<int>")
+                        help="the max job number runing at the same time. (default: all of the jobfile, max 1000)", metavar="<int>")
     common.add_argument("-s", "--startline", type=int,
-                        help="which line number(1-base) be used for the first job tesk. default: 1", metavar="<int>", default=1)
+                        help="which line number(1-base) be used for the first job. (default: 1)", metavar="<int>", default=1)
     common.add_argument("-e", "--endline", type=int,
-                        help="which line number (include) be used for the last job tesk. default: all in your job file", metavar="<int>")
+                        help="which line number (include) be used for the last job. (default: last line of the jobfile)", metavar="<int>")
     common.add_argument('-d', '--debug', action='store_true',
-                        help='log debug info', default=False)
+                        help='log debug info.', default=False)
     common.add_argument("-l", "--log", type=str,
-                        help='append log info to file, default: stdout', metavar="<file>")
-    common.add_argument('-r', '--resub', help="rebsub you job when error, 0 or minus means do not re-submit, default: 0",
+                        help='append log info to file. (default: stdout)', metavar="<file>")
+    common.add_argument('-r', '--resub', help="rebsub you job when error, 0 or minus means do not re-submit. (default: 0)",
                         type=int, default=0, metavar="<int>")
-    common.add_argument('-ivs', '--resubivs', help="rebsub interval seconds, default: 2",
+    common.add_argument('-ivs', '--resubivs', help="rebsub interval seconds. (default: 2)",
                         type=int, default=2, metavar="<int>")
-    common.add_argument('--rate', help="rate limite for job status checking per second, default: 3",
-                        type=float, default=3, metavar="<float>")
     common.add_argument("-f", "--force", default=False, action="store_true",
-                        help="force to submit jobs even if already successed")
+                        help="force to submit jobs even if already successed.")
     common.add_argument("--local", default=False, action="store_true",
-                        help="submit your jobs in localhost, same as '--mode local'")
+                        help="submit your jobs in localhost, same as '--mode local'.")
     common.add_argument("--strict", action="store_true", default=False,
-                        help="use strict to run. Means if any errors, clean all jobs and exit.")
-    common.add_argument('-v', '--version',
-                        action='version', version="v" + __version__)
+                        help="use strict to run, means if any errors, clean all jobs and exit.")
+    common.add_argument('--max-check', help="maximal number of job status checks per second, default is 3, fractions allowed. (default: 3)",
+                        type=float, default=3, metavar="<float>")
+    common.add_argument('--max-submit', help="maximal number of sge jobs submited per second, default is 30, fractions allowed. (default: 30)",
+                        type=float, default=30, metavar="<float>")
     return p
 
 
 def runsgeArgparser():
     parser = argparse.ArgumentParser(
-        description="For multi-run your shell scripts localhost, qsub or BatchCompute.", parents=[common_parser()])
-    parser.add_argument("-wd", "--workdir", type=str, help="work dir, default: %s" %
+        description="%(prog)s is a tool for managing parallel jobs from a specific shell scripts runing in localhost, SGE or BatchCompute.", parents=[common_parser()])
+    parser.add_argument("-wd", "--workdir", type=str, help="work dir. (default: %s)" %
                         os.path.abspath(os.getcwd()), default=os.path.abspath(os.getcwd()), metavar="<workdir>")
     parser.add_argument("-N", "--jobname", type=str,
-                        help="job name, default: basename(jobfile)", metavar="<jobname>")
+                        help="job name. (default: basename of the jobfile)", metavar="<jobname>")
     parser.add_argument("-lg", "--logdir", type=str,
-                        help='the output log dir, default: "%s/runjob_*_log_dir"' % os.getcwd(), metavar="<logdir>")
+                        help='the output log dir. (default: "%s/runjob_*_log_dir")' % os.getcwd(), metavar="<logdir>")
     parser.add_argument("-g", "--groups", type=int, default=1,
-                        help="groups number of lines to a new jobs, default: 1", metavar="<int>")
-    parser.add_argument('--init', help="command before all jobs, will be running in localhost",
+                        help="groups number of lines to a new jobs. (default: 1)", metavar="<int>")
+    parser.add_argument('--init', help="command before all jobs, will be running in localhost.",
                         type=str,  metavar="<cmd>")
-    parser.add_argument('--call-back', help="command after all jobs, will be running in localhost",
+    parser.add_argument('--call-back', help="command after all jobs finished, will be running in localhost.",
                         type=str,  metavar="<cmd>")
     parser.add_argument('--mode', type=str, default="sge", choices=[
-                        "sge", "local", "localhost", "batchcompute"], help="the mode to submit your jobs, default: sge, if no sge installed, always localhost.")
+                        "sge", "local", "localhost", "batchcompute"], help="the mode to submit your jobs, if no sge installed, always localhost. (default: sge)")
     parser.add_argument('-ini', '--ini',
                         help="input configfile for configurations search.", metavar="<configfile>")
     parser.add_argument("-config", '--config',   action='store_true',
                         help="show configurations and exit.",  default=False)
     sge = parser.add_argument_group("sge arguments")
-    sge.add_argument("-q", "--queue", type=str, help="the queue your job running, multi queue can be sepreated by whitespace, default: all accessed queue",
+    sge.add_argument("-q", "--queue", type=str, help="the queue your job running, multi queue can be sepreated by whitespace. (default: all accessed queue)",
                      nargs="*", metavar="<queue>")
     sge.add_argument("-m", "--memory", type=int,
-                     help="the memory used per command (GB), default: 1", default=1, metavar="<int>")
+                     help="the memory used per command (GB). (default: 1)", default=1, metavar="<int>")
     sge.add_argument("-c", "--cpu", type=int,
-                     help="the cpu numbers you job used, default: 1", default=1, metavar="<int>")
+                     help="the cpu numbers you job used. (default: 1)", default=1, metavar="<int>")
     batchcmp = parser.add_argument_group("batchcompute arguments")
     batchcmp.add_argument("-om", "--out-maping", type=str,
-                          help='the oss output directory if your mode is "batchcompute", all output file will be mapping to you OSS://BUCKET-NAME. if not set, any output will be reserved', metavar="<dir>")
+                          help='the oss output directory if your mode is "batchcompute", all output file will be mapping to you OSS://BUCKET-NAME. if not set, any output will be reserved.', metavar="<dir>")
     batchcmp.add_argument('--access-key-id', type=str,
-                          help="AccessKeyID while access oss", metavar="<str>")
+                          help="AccessKeyID while access oss.", metavar="<str>")
     batchcmp.add_argument('--access-key-secret', type=str,
-                          help="AccessKeySecret while access oss", metavar="<str>")
-    batchcmp.add_argument('--regin', type=str, default="BEIJING", choices=['BEIJING', 'HANGZHOU', 'HUHEHAOTE', 'SHANGHAI',
-                                                                           'ZHANGJIAKOU', 'CHENGDU', 'HONGKONG', 'QINGDAO', 'SHENZHEN'], help="batch compute regin, default: BEIJING")
+                          help="AccessKeySecret while access oss.", metavar="<str>")
+    batchcmp.add_argument('--region', type=str, default="beijing", choices=['beijing', 'hangzhou', 'huhehaote', 'shanghai',
+                                                                           'zhangjiakou', 'chengdu', 'hongkong', 'qingdao', 'shenzhen'], help="batch compute region. (default: beijing)")
     return parser
 
 
 def runjobArgparser():
     parser = argparse.ArgumentParser(
-        description="For manger submit your jobs from a job file to localhost or SGE cluster.",  parents=[common_parser()])
-    parser.add_argument('-i', '--injname', help="job names you need to run, default: all jobnames of you job file",
+        description="%(prog)s is a tool for managing parallel jobs from a job file running in localhost or SGE cluster.",  parents=[common_parser()])
+    parser.add_argument('-i', '--injname', help="job names you need to run. (default: all job names of the jobfile)",
                         nargs="*", type=str, metavar="<str>")
     parser.add_argument("-m", '--mode', type=str, default="sge", choices=[
-                        "sge", "local", "localhost"], help="the mode to submit your jobs, default: sge, if no sge installed, always localhost.")
+                        "sge", "local", "localhost"], help="the mode to submit your jobs, if no sge installed, always localhost. (default: sge)")
     return parser
 
 
 def shellJobArgparser(arglist):
     parser = argparse.ArgumentParser(add_help=False)
     parser.add_argument("-q", "--queue", type=str, nargs="*")
     parser.add_argument("-m", "--memory", type=int)
```

## Comparing `runjob-2.10.4.dist-info/LICENSE` & `runjob-2.10.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `runjob-2.10.4.dist-info/METADATA` & `runjob-2.10.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runjob
-Version: 2.10.4
+Version: 2.10.5
 Home-page: https://github.com/yodeng/runjob
 Author: yodeng
 Author-email: yodeng@tju.edu.cn
 License: MIT
 Requires-Python: >=2.7.10, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

