# Comparing `tmp/RecruitPlotEasy-3.0.9.tar.gz` & `tmp/RecruitPlotEasy-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RecruitPlotEasy-3.0.9.tar", last modified: Wed Nov  2 17:01:26 2022, max compression
+gzip compressed data, was "RecruitPlotEasy-3.1.0.tar", last modified: Wed Apr 12 17:48:06 2023, max compression
```

## Comparing `RecruitPlotEasy-3.0.9.tar` & `RecruitPlotEasy-3.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2022-11-02 17:01:26.425153 RecruitPlotEasy-3.0.9/
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      243 2022-11-02 17:01:26.425153 RecruitPlotEasy-3.0.9/PKG-INFO
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2022-11-02 15:17:49.000000 RecruitPlotEasy-3.0.9/README.md
-drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2022-11-02 17:01:26.351092 RecruitPlotEasy-3.0.9/RecruitPlotEasy.egg-info/
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      243 2022-11-02 17:01:26.000000 RecruitPlotEasy-3.0.9/RecruitPlotEasy.egg-info/PKG-INFO
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      725 2022-11-02 17:01:26.000000 RecruitPlotEasy-3.0.9/RecruitPlotEasy.egg-info/SOURCES.txt
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)        1 2022-11-02 17:01:26.000000 RecruitPlotEasy-3.0.9/RecruitPlotEasy.egg-info/dependency_links.txt
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)       92 2022-11-02 17:01:26.000000 RecruitPlotEasy-3.0.9/RecruitPlotEasy.egg-info/entry_points.txt
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)       28 2022-11-02 17:01:26.000000 RecruitPlotEasy-3.0.9/RecruitPlotEasy.egg-info/requires.txt
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)       10 2022-11-02 17:01:26.000000 RecruitPlotEasy-3.0.9/RecruitPlotEasy.egg-info/top_level.txt
-drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2022-11-02 17:01:26.382333 RecruitPlotEasy-3.0.9/rpe2_code/
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)       24 2022-11-02 16:46:51.000000 RecruitPlotEasy-3.0.9/rpe2_code/__init__.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)     9463 2022-11-02 16:49:52.000000 RecruitPlotEasy-3.0.9/rpe2_code/recruit_plot_easy_2_database.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)    33071 2022-11-02 15:45:17.000000 RecruitPlotEasy-3.0.9/rpe2_code/recruit_plot_easy_2_plot.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      523 2022-11-02 16:48:22.000000 RecruitPlotEasy-3.0.9/rpe2_code/rpe2_main.py
-drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2022-11-02 17:01:26.425153 RecruitPlotEasy-3.0.9/rpe2_code/supports/
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2022-11-02 16:51:28.000000 RecruitPlotEasy-3.0.9/rpe2_code/supports/__init__.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      996 2022-09-28 14:43:48.000000 RecruitPlotEasy-3.0.9/rpe2_code/supports/agnostic_reader.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)    42849 2022-10-18 17:21:08.000000 RecruitPlotEasy-3.0.9/rpe2_code/supports/bam_parser.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2169 2022-10-18 17:21:28.000000 RecruitPlotEasy-3.0.9/rpe2_code/supports/blast_parser.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)     1033 2022-09-28 19:11:20.000000 RecruitPlotEasy-3.0.9/rpe2_code/supports/cig_parser.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      991 2022-09-30 16:44:49.000000 RecruitPlotEasy-3.0.9/rpe2_code/supports/fasta_reader.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2282 2022-09-30 16:43:46.000000 RecruitPlotEasy-3.0.9/rpe2_code/supports/file_checker.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      418 2022-09-28 16:56:11.000000 RecruitPlotEasy-3.0.9/rpe2_code/supports/mdz_parser.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)    12171 2022-10-04 16:52:56.000000 RecruitPlotEasy-3.0.9/rpe2_code/supports/protein_predictor.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2595 2022-10-18 17:21:16.000000 RecruitPlotEasy-3.0.9/rpe2_code/supports/sam_parser.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)       38 2022-11-02 17:01:26.425153 RecruitPlotEasy-3.0.9/setup.cfg
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      683 2022-11-02 17:00:51.000000 RecruitPlotEasy-3.0.9/setup.py
+drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-04-12 17:48:06.495745 RecruitPlotEasy-3.1.0/
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      243 2023-04-12 17:48:06.495745 RecruitPlotEasy-3.1.0/PKG-INFO
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2022-11-02 15:17:49.000000 RecruitPlotEasy-3.1.0/README.md
+drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-04-12 17:48:06.306390 RecruitPlotEasy-3.1.0/RecruitPlotEasy.egg-info/
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      243 2023-04-12 17:48:05.000000 RecruitPlotEasy-3.1.0/RecruitPlotEasy.egg-info/PKG-INFO
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      725 2023-04-12 17:48:06.000000 RecruitPlotEasy-3.1.0/RecruitPlotEasy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)        1 2023-04-12 17:48:05.000000 RecruitPlotEasy-3.1.0/RecruitPlotEasy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)       92 2023-04-12 17:48:05.000000 RecruitPlotEasy-3.1.0/RecruitPlotEasy.egg-info/entry_points.txt
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)       28 2023-04-12 17:48:06.000000 RecruitPlotEasy-3.1.0/RecruitPlotEasy.egg-info/requires.txt
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)       10 2023-04-12 17:48:06.000000 RecruitPlotEasy-3.1.0/RecruitPlotEasy.egg-info/top_level.txt
+drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-04-12 17:48:06.353253 RecruitPlotEasy-3.1.0/rpe2_code/
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)       24 2022-11-02 16:46:51.000000 RecruitPlotEasy-3.1.0/rpe2_code/__init__.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)    11443 2023-04-12 16:57:43.000000 RecruitPlotEasy-3.1.0/rpe2_code/recruit_plot_easy_2_database.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)    34597 2023-04-12 17:31:40.000000 RecruitPlotEasy-3.1.0/rpe2_code/recruit_plot_easy_2_plot.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      630 2023-04-11 18:45:19.000000 RecruitPlotEasy-3.1.0/rpe2_code/rpe2_main.py
+drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-04-12 17:48:06.495745 RecruitPlotEasy-3.1.0/rpe2_code/supports/
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2022-11-02 16:51:28.000000 RecruitPlotEasy-3.1.0/rpe2_code/supports/__init__.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      996 2022-09-28 14:43:48.000000 RecruitPlotEasy-3.1.0/rpe2_code/supports/agnostic_reader.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)    42852 2023-04-11 18:28:56.000000 RecruitPlotEasy-3.1.0/rpe2_code/supports/bam_parser.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2169 2023-04-11 18:27:57.000000 RecruitPlotEasy-3.1.0/rpe2_code/supports/blast_parser.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)     1033 2022-09-28 19:11:20.000000 RecruitPlotEasy-3.1.0/rpe2_code/supports/cig_parser.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      991 2022-09-30 16:44:49.000000 RecruitPlotEasy-3.1.0/rpe2_code/supports/fasta_reader.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2425 2023-04-12 16:58:55.000000 RecruitPlotEasy-3.1.0/rpe2_code/supports/file_checker.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      418 2022-09-28 16:56:11.000000 RecruitPlotEasy-3.1.0/rpe2_code/supports/mdz_parser.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)    12522 2022-11-02 20:26:01.000000 RecruitPlotEasy-3.1.0/rpe2_code/supports/protein_predictor.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2597 2023-04-11 18:30:05.000000 RecruitPlotEasy-3.1.0/rpe2_code/supports/sam_parser.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)       38 2023-04-12 17:48:06.495745 RecruitPlotEasy-3.1.0/setup.cfg
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      682 2023-04-12 17:36:48.000000 RecruitPlotEasy-3.1.0/setup.py
```

### Comparing `RecruitPlotEasy-3.0.9/RecruitPlotEasy.egg-info/SOURCES.txt` & `RecruitPlotEasy-3.1.0/RecruitPlotEasy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.0.9/rpe2_code/recruit_plot_easy_2_database.py` & `RecruitPlotEasy-3.1.0/rpe2_code/recruit_plot_easy_2_database.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,31 @@
+'''
 from .supports.bam_parser import bam_parser
 from .supports.sam_parser import sam_parser
 from .supports.blast_parser import blast_parser
 
 from .supports.file_checker import file_checker
 from .supports.fasta_reader import read_fasta
 from .supports.protein_predictor import pyrodigal_manager
+'''
+
+from supports.bam_parser import bam_parser
+from supports.sam_parser import sam_parser
+from supports.blast_parser import blast_parser
+
+from supports.file_checker import file_checker
+from supports.fasta_reader import read_fasta
+from supports.protein_predictor import pyrodigal_manager
 
 import sqlite3 as sq
 import numpy as np
 
 import argparse
 import sys
+import os
 
 def convert_array(bytestring):
 	return np.frombuffer(bytestring, dtype = np.int32)
 
 
 class rpe_database_builder:
 	def __init__(self, database_path):
@@ -155,14 +166,17 @@
 		target_ref = {}
 		tr_num = 0
 		
 		print("Adding reads.")
 		reads_added = 0
 				
 		for grouping in parser:
+			if grouping is None:
+				continue
+				
 			next_set = []
 			#One result looks like so
 			#[query, target, pct_id_local, pct_id_global, pct_alignment, covered_ranges]
 			
 			query_gen = '"'+grouping[0]+'"'
 			tgt_gen = '"'+grouping[1]+'"'
 			
@@ -180,15 +194,15 @@
 
 			if tgt_gen not in seen_genomes:
 				seen_genomes[tgt_gen] = max_aln
 			else:
 				if max_aln > seen_genomes[tgt_gen]:
 					seen_genomes[tgt_gen] = max_aln
 			
-			local, glob, pctaln = grouping[2]*100, grouping[3]*100, grouping[4]*100
+			local, glob, pctaln = grouping[2], grouping[3], grouping[4]
 			
 			for tuple in grouping[5]:
 				start, stop = tuple[0], tuple[1]
 				next_set = (curq, curt, local, glob, pctaln, start, stop)
 				to_add.append(next_set)
 				
 			
@@ -233,53 +247,104 @@
 def build_opts():
 	parser = argparse.ArgumentParser(formatter_class=argparse.RawTextHelpFormatter,
 			description='''
 	''')
 	parser.add_argument('-g', '--genome',  dest = 'genome', default = None, 
 	help =  'A path to a genome in nt FASTA format.')
 	
+	parser.add_argument('-gf', '--genome_file',  dest = 'gf', default = None, 
+	help =  'A file containing a list of FASTA-format genomes, one per line. Do not use with --genome at the same time.')
+	
 	parser.add_argument('--mag',  dest = 'is_mag', action = 'store_true', 
-	help =  'Genomes file to add is a MAG: all sequences in this file will be treated as one genome.')
+	help =  'Any genomes to add are MAGs: all sequences in each genome file will be treated as the contigs of one genome.')
 	
 	parser.add_argument('--predict',  dest = 'predict', action = 'store_true', 
-	help =  'Predict proteins for the genome file.')
+	help =  'Predict proteins for each genome file.')
 	
 	parser.add_argument('-r', '--reads',  dest = 'reads', default = None, 
 	help =  'A path to a set of aligned nt reads in SAM, BAM, or tabular BLAST format.')
 	
+	parser.add_argument('-rf', '--reads_file',  dest = 'rf', default = None, 
+	help =  'A file containing a list of aligned nt reads in SAM, BAM, or tabular BLAST format, one set of reads per line. Do not use with --reads at the same time.')
+	
 	parser.add_argument('-d', '--database',  dest = 'db', default = None, 
 	help =  'Path to the database to create. Required.')
 	
 	args, unknown = parser.parse_known_args()
 	
 	return parser, args
+
+def load_file_paths(list_file):
+	file_paths = []
+	with open(list_file) as fh:
+		for line in fh:
+			cleaned = line.strip()
+			if os.path.exists(cleaned):
+				file_paths.append(cleaned)
+			else:
+				print("Can't find file:", cleaned, "skipping this file.")
+	return file_paths
 	
 def run_build():
 	parser, opts = build_opts()
 	if len(sys.argv) < 3:
 		parser.print_help()
 		sys.exit()
 	
 	genome = opts.genome
 	is_mag = opts.is_mag
 	pred = opts.predict
 	reads = opts.reads
 	db = opts.db
 	
+	gf = opts.gf
+	rf = opts.rf
+	
+	if gf is not None:
+		gf_paths = load_file_paths(gf)
+		if len(gf_paths) == 0:
+			gf_paths = None
+	else:
+		gf_paths = None
+	if rf is not None:
+		rf_paths = load_file_paths(rf)
+		if len(rf_paths) == 0:
+			rf_paths = None
+	else:
+		rf_paths = None
+	
+	if reads is not None and rf_paths is not None:
+		sys.exit("Use either --reads or --reads_file, not both.")
+		
+	if genome is not None and gf_paths is not None:
+		sys.exit("Use either --genomes or --genome_file, not both.")
+	
 	if db is None:
 		sys.exit("You need to specify a database.")
 		
-	if reads is None and genome is None:
-		sys.exit("You need to supply at least one of --reads, --genome")
+	if reads is None and genome is None and gf_paths is None and rf_paths is None:
+		sys.exit("You need to supply at least one of --reads, --genome, --reads_file, or --genome_file")
+	
 	
 	mn = rpe_database_builder(db)
 	mn.open()
 	
 	if reads is not None:
 		mn.add_reads_to_db(reads)
+	
+	if rf_paths is not None:
+		for read_file in rf_paths:
+			mn.add_reads_to_db(read_file)
 
 	if genome is not None:
 		mn.add_genomes_to_db_from_file(file = genome, 
 										is_mag = is_mag, 
 										predict = pred)	
+										
+	if gf_paths is not None:
+		for genome_file in gf_paths:
+			mn.add_genomes_to_db_from_file(file = genome_file, 
+										is_mag = is_mag, 
+										predict = pred)
+			
 	mn.close()
```

### Comparing `RecruitPlotEasy-3.0.9/rpe2_code/recruit_plot_easy_2_plot.py` & `RecruitPlotEasy-3.1.0/rpe2_code/recruit_plot_easy_2_plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 import argparse
 
 import multiprocessing
 
 class rpdb:
 	def __init__(self, db, id_cut = 95, id_step = 0.5, gen_step = 1000,
-				criteria = "local", id_measure = "local", do_prot = False):
+				criteria = "local", id_measure = "local", do_prot = False,
+				output_base = "recruitment_plots"):
 		
 		self.db = db
 		self.conn = None
 		self.curs = None
 		
 		self.samples = None
 		self.genomes = None
@@ -52,14 +53,15 @@
 		self.y_max = 100
 		
 		self.id_cutoff = id_cut
 		
 		self.y_step = id_step
 		self.x_step = gen_step
 		
+		self.outbase = output_base
 		self.recplot = None
 
 	def open(self):
 		self.conn = sq.connect(self.db)
 		self.curs = self.conn.cursor()
 		
 	def close(self):
@@ -217,17 +219,17 @@
 							returns_by_bin[start_bin] = to_add - 1
 						
 						s = current_end
 						
 		return returns_by_bin
 	
 	def load_sample(self):
-		if not os.path.exists("recruitment_plots"):
-			os.mkdir("recruitment_plots")
-		this_samp = os.path.normpath("recruitment_plots/"+self.current_sample)
+		if not os.path.exists(self.outbase):
+			os.mkdir(self.outbase)
+		this_samp = os.path.normpath(self.outbase+"/"+self.current_sample)
 		if not os.path.exists(this_samp):
 			os.mkdir(this_samp)
 	
 		num_ybins = int((self.y_max-self.y_min) / self.y_step)+1
 		
 		self.y_bins = np.linspace(self.y_min, self.y_max, num = num_ybins, dtype = np.float_)
 		
@@ -305,23 +307,25 @@
 							#cut = self.id_cutoff,
 							id_step = self.y_step,
 							genome_step = self.x_step,
 							contig_sizes = self.contig_lens_by_id,
 							protein_info = protein_subset,
 							contig_name_dict = self.mag_contig_ids,
 							mag_name = self.current_mag,
-							sample = self.current_sample) 
+							sample = self.current_sample,
+							outdir = self.outbase) 
 		
 		self.recplot.build()
 	
 class recplot:
 	def __init__(self, data, y, 
 				#cut, 
 				id_step, genome_step, contig_sizes, protein_info, 
-				contig_name_dict, tad = 80, mag_name = None, sample = None):
+				contig_name_dict, tad = 80, mag_name = None, sample = None,
+				outdir = "recruitment_plots"):
 		
 		self.raw_data = data
 		self.contig_sizes = contig_sizes
 		self.gen_step = genome_step
 		#Flip k-v
 		self.ct_dict = dict([value, key] for key, value in contig_name_dict.items())
 		self.ct_names = None
@@ -367,21 +371,22 @@
 		self.upper_right_in = None
 		self.upper_right_out = None
 		#In-grp histogram local maxima here
 		self.peaks = None
 		
 		self.lower_right_data = None
 		
+		self.output_base = outdir
 
 		self.sample = sample
 		self.mag = mag_name
 		if self.do_prot:
-			self.plot_name = os.path.normpath("recruitment_plots/" +self.sample + "/" + mag_name + "_proteins_recruitment_plot.html")
+			self.plot_name = os.path.normpath(self.output_base + "/" +self.sample + "/" + mag_name + "_proteins_recruitment_plot.html")
 		else:
-			self.plot_name = os.path.normpath("recruitment_plots/" +self.sample + "/" + mag_name + "_recruitment_plot.html")
+			self.plot_name = os.path.normpath(self.output_base + "/" +self.sample + "/" + mag_name + "_recruitment_plot.html")
 	
 	#Data comes in as a per-base count 
 	def bin_raw(self):
 		print("Processing", self.mag)
 		self.data = {}
 		self.bin_left = {}
 		self.bin_right = {}
@@ -680,373 +685,388 @@
 		self.tad_in = self.tad_values[lowest_avail]
 
 		#top right chart
 		max_obs = max([max(self.upper_left_in), max(self.upper_left_out)])
 		
 		self.depth_hist_breaks = np.linspace(0, max_obs, num = 199)
 		#reuse depth chart info
+		
 		self.upper_right_in =  np.histogram(self.upper_left_in, bins = self.depth_hist_breaks)[0]
 		self.upper_right_out = np.histogram(self.upper_left_out, bins = self.depth_hist_breaks)[0]
 		
+		#self.upper_right_in = np.histogram(np.log10(self.upper_left_in), bins = self.depth_hist_breaks)[0]
+		#self.upper_right_out = np.histogram(self.upper_left_out, bins = self.depth_hist_breaks)[0]
+		#self.upper_right_in[self.upper_right_in == 0] = 0.01
+		#self.upper_right_out[self.upper_right_out==0] = 0.01
+		#self.upper_right_in = np.log10(self.upper_right_in)
+		#self.upper_right_out = np.log10(self.upper_right_out)
+		
 	def make_plots(self):
 		print("Plotting", self.mag)
 		max_bin_count = self.data.max()
-		min_bin_count = self.data[np.nonzero(self.data)].min()
-		#order of magnitude
-		
-		#smallest oom is this
-		current_oom = -len(str(int(1/min_bin_count))) + 1
-		
-		#current_oom = 0
-		tick_positions = []
-		
-		while min_bin_count < max_bin_count:
-			tick_positions.append(current_oom)
-			min_bin_count *= 10
-			current_oom += 1
-
-		tick_labels = []
-		for oom in tick_positions:
-			tick_labels.append("10e"+str(oom))
-		
-		#'#1f77b4' is a medium blue
-		#'#ff7f0e' is a burnt orange
-		#These are colorblind friendly contrasts.
-		
-		overall_plot =  make_subplots(rows=3, cols=2, 
-									column_widths=[0.66, 0.34], 
-									row_heights = [0.30, 0.10, 0.60],
-
-									shared_xaxes=True,
-									shared_yaxes=True,
-									horizontal_spacing = 0.025,
-									vertical_spacing = 0.035)
-		
-		#This one is strange
-		#The protein hovertext needs multiple lines, but the customdata
-		#arg doesn't appear to work for customdata of more than 1 row
-		#Therefore we just <br>.join() a list of text as the labels.
-		annot_hov = "{text}"
-			
-		#Protein independent hover templates
-		bot_left_hov = 	"Position in Genome: %{x:0d}<br>" +\
-						"Percent Identity: %{y:}%<br>" +\
-						"Log 10 Base Count: %{z:.4f}<br>" +\
+		if max_bin_count < 1: #i.e. max bin == 0, guarantee this with floats by using 1 as the inequality
+			#min_bin_count = 1
+			print("No best-hit reads were found for", self.mag)
+			print("There is no information to plot for this genome under your current settings. This genome will be skipped.")
+			
+		else:
+			min_bin_count = self.data[np.nonzero(self.data)].min()
+
+			#order of magnitude
+			#smallest oom is this
+			current_oom = -len(str(int(1/min_bin_count))) + 1
+			
+			#current_oom = 0
+			tick_positions = []
+			
+			while min_bin_count < max_bin_count:
+				tick_positions.append(current_oom)
+				min_bin_count *= 10
+				current_oom += 1
+
+			tick_labels = []
+			for oom in tick_positions:
+				tick_labels.append("10e"+str(oom))
+			
+			#'#1f77b4' is a medium blue
+			#'#ff7f0e' is a burnt orange
+			#These are colorblind friendly contrasts.
+			
+			overall_plot =  make_subplots(rows=3, cols=2, 
+										column_widths=[0.66, 0.34], 
+										row_heights = [0.30, 0.10, 0.60],
+
+										shared_xaxes=True,
+										shared_yaxes=True,
+										horizontal_spacing = 0.025,
+										vertical_spacing = 0.035)
+			
+			#This one is strange
+			#The protein hovertext needs multiple lines, but the customdata
+			#arg doesn't appear to work for customdata of more than 1 row
+			#Therefore we just <br>.join() a list of text as the labels.
+			annot_hov = "{text}"
+				
+			#Protein independent hover templates
+			bot_left_hov = 	"Position in Genome: %{x:0d}<br>" +\
+							"Percent Identity: %{y:}%<br>" +\
+							"Log 10 Base Count: %{z:.4f}<br>" +\
+							"<extra></extra>"
+									
+			#hover data templates
+			in_dep_hov = "Position in Genome: %{x:0d}<br>" +\
+						"Avg. Within-Pop. Depth: %{y:.2f}" +\
 						"<extra></extra>"
+
+			out_dep_hov = "Position in Genome: %{x:0d}<br>" +\
+						"Avg. Outside-Pop. Depth: %{y:.2f}" +\
+						"<extra></extra>"
+										
+			#Protein independent hover templates
+			bot_right_hov = "Total Bases: %{x:0d}<br>" +\
+								"Percent Identity: %{y:}%<br>" + \
+								"<extra></extra>"
 								
-		#hover data templates
-		in_dep_hov = "Position in Genome: %{x:0d}<br>" +\
-					"Avg. Within-Pop. Depth: %{y:.2f}" +\
-					"<extra></extra>"
-
-		out_dep_hov = "Position in Genome: %{x:0d}<br>" +\
-					"Avg. Outside-Pop. Depth: %{y:.2f}" +\
-					"<extra></extra>"
-									
-		#Protein independent hover templates
-		bot_right_hov = "Total Bases: %{x:0d}<br>" +\
-							"Percent Identity: %{y:}%<br>" + \
-							"<extra></extra>"
-							
-							
-		#TAD *could* have protein info, but I don't think it bears a fourth repetition
-		tad_hov = "Contig: %{x:c}<br>" +\
-					"TAD Level: %{y:c}<br>" +\
-					"Depth: %{z:.2f}" +\
-					"<extra></extra>"
-					
-		
-		top_right_hov_in = "Count of Obs.: %{x:0d}<br>" +\
-		"Avg. Within-Pop. Depth: %{y:.4f}<br>" +\
-		"<extra></extra>"
-		
-		top_right_hov_out = "Count of Obs.: %{x:0d}<br>" +\
-		"Avg. Outside-Pop. Depth: %{y:.4f}<br>" +\
-		"<extra></extra>"
-		
-		#bot left main plot
-		#Needs to have labels added.
-		overall_plot.add_trace(go.Heatmap(z=np.log10(self.data), 
-								x = self.bin_mids,
-								y = self.y,
-								colorbar = dict(
-									x = -0.1,
-									tickvals = tick_positions,
-									ticktext = tick_labels
-									),
-								colorscale="blues",
-								hovertemplate = bot_left_hov
-								),
-								row = 3, col = 1)
-		
-		#bot right - only one of these
-		overall_plot.add_trace(go.Bar(x = self.lower_right_data, 
-								y = self.y,
-								orientation='h',
-								marker = dict(color = '#1f77b4'),
-								hovertemplate = bot_right_hov
-								),
-								row = 3, col = 2)
-		
-		#text_rec = []
-		
-		#We just use the protein labels as a repo - normally it would be filled out
-		if not self.do_prot:
-			self.protein_labels = []
-			for c, s, e in zip(self.ct_names, self.bin_left, self.bin_right):
-				next_label = "<br>".join(["Contig: " + c,
-										"Genome Region: " + str(s) + "-" + str(e)
-										])
-				self.protein_labels.append(next_label)
-		
-		overall_plot.add_trace(go.Scatter(x = self.bin_mids,
-								y = [1] * len(self.bin_mids),
-								text = self.protein_labels,
-								marker = dict(color = '#1f77b4'),
-								hoverinfo = "text"
-								),
-								row = 2, col = 1)
 								
-		which_viz = None
-		which_id = None
-		has_default = False
-		group = 0
-		
-		starting_step = len(overall_plot.data)
-		
-		step_groups = {}
-		id_grp = {}
-		
-		
-		tad_ticks = np.linspace(0, self.tad_max, num = 5, dtype = int).tolist()
-		#tad_labels = 
-		tad_colorbar = dict(tickvals = tad_ticks)
-		
-		#Here, we iterate over the in-groups to add traces for each pct id in-group.
-		for pct_id_cutoff in self.y:
-			self.cutoff = pct_id_cutoff
-			#recalculate data
-			self.top_half()
+			#TAD *could* have protein info, but I don't think it bears a fourth repetition
+			tad_hov = "Contig: %{x:c}<br>" +\
+						"TAD Level: %{y:c}<br>" +\
+						"Depth: %{z:.2f}" +\
+						"<extra></extra>"
+						
 			
-			idname = str(pct_id_cutoff)
+			top_right_hov_in = "Count of Obs.: %{x:0d}<br>" +\
+			"Avg. Within-Pop. Depth: %{y:.4f}<br>" +\
+			"<extra></extra>"
+			
+			top_right_hov_out = "Count of Obs.: %{x:0d}<br>" +\
+			"Avg. Outside-Pop. Depth: %{y:.4f}<br>" +\
+			"<extra></extra>"
+			
+			#bot left main plot
+			#Needs to have labels added.
+			overall_plot.add_trace(go.Heatmap(z=np.log10(self.data), 
+									x = self.bin_mids,
+									y = self.y,
+									colorbar = dict(
+										x = -0.1,
+										tickvals = tick_positions,
+										ticktext = tick_labels
+										),
+									colorscale="blues",
+									hovertemplate = bot_left_hov
+									),
+									row = 3, col = 1)
 			
-			#print(pct_id_cutoff, self.tad_in, self.cov_in)
+			#bot right - only one of these
+			overall_plot.add_trace(go.Bar(x = self.lower_right_data, 
+									y = self.y,
+									orientation='h',
+									marker = dict(color = '#1f77b4'),
+									hovertemplate = bot_right_hov
+									),
+									row = 3, col = 2)
 			
-			step_groups[pct_id_cutoff] = [starting_step,
-										starting_step + 1,
-										starting_step + 2,
-										starting_step + 3,
-										starting_step + 4]
-										#starting_step + 5,]
-										
-			starting_step += 5
-											
-			#Set the only default line *near* 95 pct id.
-			if self.cutoff >= 95.0 and not has_default:
-				which_viz = group
-				which_id = pct_id_cutoff
-				has_default = True
-			else:
-				group += 1
+			#text_rec = []
 			
-			line_height = self.cutoff-(self.id_step/2)
+			#We just use the protein labels as a repo - normally it would be filled out
+			if not self.do_prot:
+				self.protein_labels = []
+				for c, s, e in zip(self.ct_names, self.bin_left, self.bin_right):
+					next_label = "<br>".join(["Contig: " + c,
+											"Genome Region: " + str(s) + "-" + str(e)
+											])
+					self.protein_labels.append(next_label)
 			
-			#top left in group
-			overall_plot.add_trace(go.Scatter(x = self.bin_mids, 
-											y = self.upper_left_in,
-											marker = dict(color = '#1f77b4'),
-											visible = False,
-											hovertemplate = in_dep_hov
-											),
-											row = 1, col = 1)
-			#top left out group							
 			overall_plot.add_trace(go.Scatter(x = self.bin_mids,
-											y = self.upper_left_out, 
-											marker = dict(color = '#ff7f0e'),
-											visible = False,
-											hovertemplate = out_dep_hov	
-											), 
-											row = 1, col = 1)
-
-			#mid right tad
-			#Update fixed colorbar, add the coverage values and this is done.
-			overall_plot.add_trace(go.Heatmap(z = self.tad_in,
-											x = self.tad_contigs,
-											y = self.tad_names,
-											visible = False,
-											hovertemplate = tad_hov,
-											colorbar = tad_colorbar,
-											zmin = 0,
-											zmax = self.tad_max*1.05
-											),
-											row = 2, col = 2)
-								
-			#top right in group default
-			overall_plot.add_trace(go.Scatter(x = self.upper_right_in, 
-			y = self.depth_hist_breaks, 
-			marker = dict(color = '#1f77b4'),
-			visible = False,
-			hovertemplate = top_right_hov_in
-			), 
-			row = 1, col = 2)
-			#top right out group default
-			overall_plot.add_trace(go.Scatter(x = self.upper_right_out, 
-			y = self.depth_hist_breaks, 
-			marker = dict(color = '#ff7f0e'),
-			visible = False,
-			hovertemplate = top_right_hov_out
-			), 
-			row = 1, col = 2)
-			
-		#Set default lines as nearest to 90
-		for i in step_groups[which_id]:
-			overall_plot.data[i].visible = True
-			
-		#in-group highlight
-		overall_plot.add_hrect(y0 = which_id-(self.id_step/2), 
-								y1 = 100+(self.id_step/2),
-								row = 3, col = 1,
-								line_width=0,
-								fillcolor="red",
-								opacity=0.13)
-								#,layer="below")
-								
-		overall_plot.add_hrect(y0 = which_id-(self.id_step/2), 
-								y1 = 100+(self.id_step/2),
-								row = 3, col = 2,
-								line_width=0,
-								fillcolor="red",
-								opacity=0.13)
-								#,layer="below")
-			
-		
-			
-		#overall_plot.add_hrect(y0 = 0, y1 = max_tad,
-		#						row = 2, col = 2)
-		
-		left_box = {'type': 'rect', 
-					'x0': 0, 
-					'x1': 1, 
-					'xref': 
-					'x3 domain', 
-					'y0': 0, 
-					'y1': 1, 
-					'yref': 'y3 domain'}
-		
-		right_box = {'type': 'rect', 
-					'x0': 0, 
-					'x1': 1, 
-					'xref': 
-					'x4 domain', 
-					'y0': 0, 
-					'y1': 1, 
-					'yref': 'y4 domain'}
-					
-		initial_shapes = list(overall_plot.layout["shapes"])
-		initial_shapes.append(left_box)
-		initial_shapes.append(right_box)
-		overall_plot.layout["shapes"] = tuple(initial_shapes)
-		
-		steps = []
-		for group in step_groups:
-			step = dict(
-					method="update",
-					args=[{"visible": [False] * len(overall_plot.data)},
-						{"shapes": [{'fillcolor': 'red',
-									#'layer': 'below',
-									'line': {'width': 0},
-									'opacity': 0.13,
-									'type': 'rect',
-									'x0': 0,
-									'x1': 1,
-									'xref': 'x5 domain',
-									'y0': group-(self.id_step/2),
-									'y1': 100+(self.id_step/2),
-									'yref': 'y5'},
-									
-									#lower right highlight
-									{'fillcolor': 'red',
-									#'layer': 'below',
-									'line': {'width': 0},
-									'opacity': 0.13,
-									'type': 'rect',
-									'x0': 0,
-									'x1': 1,
-									'xref': 'x6 domain',
-									'y0': group-(self.id_step/2),
-									'y1': 100+(self.id_step/2),
-									'yref': 'y6'},
-									
-									#mid left box
-									left_box,
-									
-									#mid right box
-									right_box
+									y = [1] * len(self.bin_mids),
+									text = self.protein_labels,
+									marker = dict(color = '#1f77b4'),
+									hoverinfo = "text"
+									),
+									row = 2, col = 1)
 									
-									]
-						}],
+			which_viz = None
+			which_id = None
+			has_default = False
+			group = 0
+			
+			starting_step = len(overall_plot.data)
+			
+			step_groups = {}
+			id_grp = {}
+			
+			
+			tad_ticks = np.linspace(0, self.tad_max, num = 5, dtype = int).tolist()
+			#tad_labels = 
+			tad_colorbar = dict(tickvals = tad_ticks)
+			
+			#Here, we iterate over the in-groups to add traces for each pct id in-group.
+			for pct_id_cutoff in self.y:
+				self.cutoff = pct_id_cutoff
+				#recalculate data
+				self.top_half()
+				
+				idname = str(pct_id_cutoff)
+				
+				#print(pct_id_cutoff, self.tad_in, self.cov_in)
+				
+				step_groups[pct_id_cutoff] = [starting_step,
+											starting_step + 1,
+											starting_step + 2,
+											starting_step + 3,
+											starting_step + 4]
+											#starting_step + 5,]
+											
+				starting_step += 5
+												
+				#Set the only default line *near* 95 pct id.
+				if self.cutoff >= 95.0 and not has_default:
+					which_viz = group
+					which_id = pct_id_cutoff
+					has_default = True
+				else:
+					group += 1
+				
+				line_height = self.cutoff-(self.id_step/2)
+				
+				#top left in group
+				overall_plot.add_trace(go.Scatter(x = self.bin_mids, 
+												y = self.upper_left_in,
+												marker = dict(color = '#1f77b4'),
+												visible = False,
+												hovertemplate = in_dep_hov
+												),
+												row = 1, col = 1)
+				#top left out group							
+				overall_plot.add_trace(go.Scatter(x = self.bin_mids,
+												y = self.upper_left_out, 
+												marker = dict(color = '#ff7f0e'),
+												visible = False,
+												hovertemplate = out_dep_hov	
+												), 
+												row = 1, col = 1)
+
+				#mid right tad
+				#Update fixed colorbar, add the coverage values and this is done.
+				overall_plot.add_trace(go.Heatmap(z = self.tad_in,
+												x = self.tad_contigs,
+												y = self.tad_names,
+												visible = False,
+												hovertemplate = tad_hov,
+												colorbar = tad_colorbar,
+												zmin = 0,
+												zmax = self.tad_max*1.05
+												),
+												row = 2, col = 2)
+				
+				#Prevent 0-depth outgroups from running away with the scale
+				#max_in_grp = self.upper_right_in.max() + 1
+				#self.upper_right_out[self.upper_right_out > max_in_grp] = max_in_grp
+				
+				#top right in group default
+				overall_plot.add_trace(go.Scatter(x = self.upper_right_in, 
+				y = self.depth_hist_breaks, 
+				marker = dict(color = '#1f77b4'),
+				visible = False,
+				hovertemplate = top_right_hov_in
+				), 
+				row = 1, col = 2)
+				#top right out group default
+				overall_plot.add_trace(go.Scatter(x = self.upper_right_out, 
+				y = self.depth_hist_breaks, 
+				marker = dict(color = '#ff7f0e'),
+				visible = False,
+				hovertemplate = top_right_hov_out
+				), 
+				row = 1, col = 2)
+				
+			#Set default lines as nearest to 90
+			for i in step_groups[which_id]:
+				overall_plot.data[i].visible = True
+				
+			#in-group highlight
+			overall_plot.add_hrect(y0 = which_id-(self.id_step/2), 
+									y1 = 100+(self.id_step/2),
+									row = 3, col = 1,
+									line_width=0,
+									fillcolor="red",
+									opacity=0.13)
+									#,layer="below")
 									
-					label = str(group)
-			)
-			#lower left and lower right data
-			step["args"][0]["visible"][0] = True
-			step["args"][0]["visible"][1] = True
-			step["args"][0]["visible"][2] = True
-			for i in step_groups[group]:
-				step["args"][0]["visible"][i] = True
+			overall_plot.add_hrect(y0 = which_id-(self.id_step/2), 
+									y1 = 100+(self.id_step/2),
+									row = 3, col = 2,
+									line_width=0,
+									fillcolor="red",
+									opacity=0.13)
+									#,layer="below")
 				
-			steps.append(step)
-			
-		id_slider = [dict(
-			#match default viz
-			active=which_viz,
-			currentvalue={"prefix": "Percent ID cutoff: ", "suffix": "%"},
-			pad={"t": 50},
-			bgcolor = '#1f77b4',
-			steps=steps
-		)]
 			
+				
+			#overall_plot.add_hrect(y0 = 0, y1 = max_tad,
+			#						row = 2, col = 2)
 			
-		overall_plot['layout']['xaxis2'].pop('matches')
+			left_box = {'type': 'rect', 
+						'x0': 0, 
+						'x1': 1, 
+						'xref': 
+						'x3 domain', 
+						'y0': 0, 
+						'y1': 1, 
+						'yref': 'y3 domain'}
+			
+			right_box = {'type': 'rect', 
+						'x0': 0, 
+						'x1': 1, 
+						'xref': 
+						'x4 domain', 
+						'y0': 0, 
+						'y1': 1, 
+						'yref': 'y4 domain'}
+						
+			initial_shapes = list(overall_plot.layout["shapes"])
+			initial_shapes.append(left_box)
+			initial_shapes.append(right_box)
+			overall_plot.layout["shapes"] = tuple(initial_shapes)
+			
+			steps = []
+			for group in step_groups:
+				step = dict(
+						method="update",
+						args=[{"visible": [False] * len(overall_plot.data)},
+							{"shapes": [{'fillcolor': 'red',
+										#'layer': 'below',
+										'line': {'width': 0},
+										'opacity': 0.13,
+										'type': 'rect',
+										'x0': 0,
+										'x1': 1,
+										'xref': 'x5 domain',
+										'y0': group-(self.id_step/2),
+										'y1': 100+(self.id_step/2),
+										'yref': 'y5'},
+										
+										#lower right highlight
+										{'fillcolor': 'red',
+										#'layer': 'below',
+										'line': {'width': 0},
+										'opacity': 0.13,
+										'type': 'rect',
+										'x0': 0,
+										'x1': 1,
+										'xref': 'x6 domain',
+										'y0': group-(self.id_step/2),
+										'y1': 100+(self.id_step/2),
+										'yref': 'y6'},
+										
+										#mid left box
+										left_box,
+										
+										#mid right box
+										right_box
+										
+										]
+							}],
+						
+						label = str(round(group, 2))
+				)
+				#lower left and lower right data
+				step["args"][0]["visible"][0] = True
+				step["args"][0]["visible"][1] = True
+				step["args"][0]["visible"][2] = True
+				for i in step_groups[group]:
+					step["args"][0]["visible"][i] = True
+					
+				steps.append(step)
+				
+			id_slider = [dict(
+				#match default viz
+				active=which_viz,
+				currentvalue={"prefix": "Percent ID cutoff: ", "suffix": "%"},
+				pad={"t": 50},
+				bgcolor = '#1f77b4',
+				steps=steps
+			)]
+				
+				
+			overall_plot['layout']['xaxis2'].pop('matches')
 
-		overall_plot['layout']['xaxis2']['showticklabels'] = True
-		
-		overall_plot['layout']['yaxis3']['showticklabels'] = False
-		overall_plot['layout']['yaxis3'].pop('matches')
-		
-		overall_plot['layout']['xaxis4'].pop('matches')
-		overall_plot['layout']['yaxis4'].pop('matches')
-		overall_plot['layout']['yaxis4']['showticklabels'] = False
-		
-		
-		#print(overall_plot['layout'])
-		
-		overall_plot.update_layout(showlegend = False)
-		overall_plot.update_layout(margin = dict(t=25))
-		overall_plot.update_xaxes(showgrid=False)
-		overall_plot.update_yaxes(showgrid=False)
-		
-		#overall_plot.update_layout(hovermode="x unified")
-		
-		overall_plot.update_layout(
-			sliders=id_slider
-		)
-		
-		#print(overall_plot)
-		#print(overall_plot['layout'])
-		
-		overall_plot.write_html(self.plot_name)
+			overall_plot['layout']['xaxis2']['showticklabels'] = True
+			
+			overall_plot['layout']['yaxis3']['showticklabels'] = False
+			overall_plot['layout']['yaxis3'].pop('matches')
+			
+			overall_plot['layout']['xaxis4'].pop('matches')
+			overall_plot['layout']['yaxis4'].pop('matches')
+			overall_plot['layout']['yaxis4']['showticklabels'] = False
+			
+			
+			#print(overall_plot['layout'])
+			
+			overall_plot.update_layout(showlegend = False)
+			overall_plot.update_layout(margin = dict(t=25))
+			overall_plot.update_xaxes(showgrid=False)
+			overall_plot.update_yaxes(showgrid=False)
+			
+			#overall_plot.update_layout(hovermode="x unified")
+			
+			overall_plot.update_layout(
+				sliders=id_slider
+			)
+			
+			#print(overall_plot)
+			#print(overall_plot['layout'])
+			
+			overall_plot.write_html(self.plot_name)
 		
 		
 	def build(self):
 		self.bin_raw()
 		self.concatenate()
-		#self.depth_chart()
-		#self.depth_histogram()
-		#self.id_histogram()
 		self.make_plots()
 		
 
 def plot_opts():
 	parser = argparse.ArgumentParser(formatter_class=argparse.RawTextHelpFormatter,
 			description='''
 	''')
@@ -1058,14 +1078,17 @@
 	
 	parser.add_argument('-w', '--width',  dest = 'width', type=int, default = 1000, 
 	help =  'Genome bin width. The genome will be divided into bins of [width] size for plotting. Def. 1000')
 	
 	parser.add_argument('-i', '--id_step',  dest = 'height', type=float, default = 0.5, 
 	help =  'Pct. ID bin height. Reads will be binned every [height] pct. ID. Default 0.5.')
 	
+	parser.add_argument('-o', '--output',  dest = 'outdir', default = "recruitment_plots", 
+	help =  'Base directory for outputs. Defaults to creating "recruitment_plots/" in the CWD.')
+	
 	args, unknown = parser.parse_known_args()
 	
 	return parser, args
 		
 def run_plot():
 	parser, opts = plot_opts()
 	db = opts.db
@@ -1075,16 +1098,17 @@
 		sys.exit()
 		
 	do_proteins = opts.prot
 	
 	width = opts.width
 	height = opts.height
 	
-
-	mn = rpdb(db, gen_step = width, id_step = height, do_prot = do_proteins)
+	out = opts.outdir
+	
+	mn = rpdb(db, gen_step = width, id_step = height, do_prot = do_proteins, output_base = out)
 	mn.open()
 	mn.parse_db()
 	
 	if do_proteins:
 		if mn.proteins is None:
 			print("No proteins have been added to this database. Quitting.")
 			mn.close()
@@ -1094,16 +1118,14 @@
 		print("Plotting proteins with pct ID height", height)
 	else:
 		print("Plotting genome with bin width ", width, 'bases and pct ID height ', height)
 	
 	
 	for sample in mn.samples:
 		mn.set_sample(sample)
-		#print(mn.mags_in_sample)
-		#print(mn.proteins.keys())
 		for mag in mn.mags_in_sample:
 			mn.set_mag(mag)
 			mn.craft_query()
 			mn.load_sample()
 		
 	mn.close()
```

### Comparing `RecruitPlotEasy-3.0.9/rpe2_code/rpe2_main.py` & `RecruitPlotEasy-3.1.0/rpe2_code/rpe2_main.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 	else:
 		action = sys.argv[1]
 		if action not in ["build", "plot"]:
 			print("I could not recognize your module:", action+".", "Please try again.")
 			sys.exit()
 		
 		if action == "build":
-			from .recruit_plot_easy_2_database import run_build
+			#from .recruit_plot_easy_2_database import run_build
+			from recruit_plot_easy_2_database import run_build
 			run_build()
 			
 		if action == "plot":
-			from .recruit_plot_easy_2_plot import run_plot
+			#from .recruit_plot_easy_2_plot import run_plot
+			from recruit_plot_easy_2_plot import run_plot
 			run_plot()
 			
 			
 if __name__ == "__main__":
 	main()
```

### Comparing `RecruitPlotEasy-3.0.9/rpe2_code/supports/agnostic_reader.py` & `RecruitPlotEasy-3.1.0/rpe2_code/supports/agnostic_reader.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.0.9/rpe2_code/supports/bam_parser.py` & `RecruitPlotEasy-3.1.0/rpe2_code/supports/bam_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -732,21 +732,21 @@
 		#Get num matches
 		parsed_mds = mdz_to_match_count(mdz_seg)
 		
 		matches, mismatches = parsed_mds.get_match_mismatch()
 		
 		total_align = matches+mismatches
 		
-		pct_id_local = matches / total_align
+		pct_id_local = (matches / total_align) * 100
 		#The second item in the last tuple of covered range is the last pos covered + 1, adjust back
 		last_pos_aligned = covered_ranges[len(covered_ranges)-1][1] - 1
 		#We don't need to pad the last pos covered
-		pct_id_global = matches / (last_pos_aligned - start)
+		pct_id_global = (matches / read_len) * 100
 		
-		pct_alignment = total_align / read_len
+		pct_alignment = (total_align / read_len) * 100
 		'''
 		as_np_list = []
 		for tuple in covered_ranges:
 			for index in tuple:
 				as_np_list.append(index)
 		covered_ranges = np.array(as_np_list, dtype = np.int32)
 		'''
@@ -757,16 +757,15 @@
 		bam_record = self.handle.next()
 		
 		if bam_record:
 			line = self.parse_bam_entry(bam_record)
 			return line
 		else:
 			raise StopIteration
-		
-		
+			
 class bam_parser:
 	def __init__(self, file):
 		self.file = file
 		self.header = []
 		self.handle = None
 		self.get_header()
```

### Comparing `RecruitPlotEasy-3.0.9/rpe2_code/supports/blast_parser.py` & `RecruitPlotEasy-3.1.0/rpe2_code/supports/blast_parser.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.0.9/rpe2_code/supports/cig_parser.py` & `RecruitPlotEasy-3.1.0/rpe2_code/supports/cig_parser.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.0.9/rpe2_code/supports/fasta_reader.py` & `RecruitPlotEasy-3.1.0/rpe2_code/supports/fasta_reader.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.0.9/rpe2_code/supports/file_checker.py` & `RecruitPlotEasy-3.1.0/rpe2_code/supports/file_checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,29 +3,35 @@
 	def __init__(self, file):
 		self.file = file
 		self.format = "Unknown"
 		
 		self.original_name = None
 		self.sqlname = None
 		self.get_sql_name()
-		
-	def get_sql_name(self):
-		base = os.path.basename(self.file)
-		self.original_name = base
-		while base != os.path.splitext(base)[0]:
-			base = os.path.splitext(base)[0]
-			
+	
+	def sql_safe(self, string):
+		#Sanitize for SQL
+		#These are chars safe for sql
 		sql_safe = set('_abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789')
-		current_chars = set(base)
+		current_chars = set(string)
 		#self.sql_name = self.basename
 		#Identify SQL-unsafe characters as those outside the permissible set and replace all with underscores.
 		for char in current_chars - sql_safe:
-			base = base.replace(char, "_")
+			string = string.replace(char, "_")
+		
+		return string
+	
+	
+	def get_sql_name(self):
+		base = os.path.basename(self.file)
+		self.original_name = base
+		#while base != os.path.splitext(base)[0]:
+		##	base = os.path.splitext(base)[0]
 		
-		self.sqlname = base
+		self.sqlname = self.sql_safe(self.original_name)
 		
 	def check_is_fasta(self):
 		fh = open(self.file, "r")
 		fmt_fine = True
 		for i in range(0, 30):
 			try:
 				line = fh.readline()
```

### Comparing `RecruitPlotEasy-3.0.9/rpe2_code/supports/protein_predictor.py` & `RecruitPlotEasy-3.1.0/rpe2_code/supports/protein_predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,14 @@
 	def convert_sequences(self, contents):
 		self.sequences = {}
 		for seq in contents:
 			name = seq.encode()
 			nt = contents[seq].encode()
 			self.sequences[name] = nt
 		
-		
 	#Collect up to the first 32 million bases for use in training seq.
 	def train_manager(self):
 		running_sum = 0
 		seqs_added = 0
 		if self.training_seq is None:
 			self.training_seq = []
 			for seq in self.sequences:
@@ -265,15 +264,19 @@
 			source = seq.decode()
 			seqname = source + "_"
 			
 			for gene in self.predicted_genes[seq]:
 				gene_name = seqname + str(count)
 				count += 1
 				renamed[gene_name] = gene.translate()
-				this_annot = (gene.strand, gene.begin, gene.end, str(gene._gene_data),)
+				#print(dir(gene))
+				annotation = ";".join(["GC:" + str(round(gene.gc_cont, 4)),
+										"Start_Type:" +gene.start_type])
+				#print(gene.strand, gene.begin, gene.end, str(gene._gene_data),)
+				this_annot = (gene.strand, gene.begin, gene.end, annotation,)
 				self.annot[gene_name] = this_annot
 				self.source_gen[gene_name] = source
 				
 		self.predicted_genes = renamed
 	
 	#Writeouts
 	def write_nt(self):
@@ -375,8 +378,15 @@
 				
 	def run_for_fastaai(self):
 		self.verbose = False
 		self.import_sequences()
 		self.train_manager()
 		self.predict_and_compare()
 		self.write_aa()
-	
+	
+#Testing section.	
+#import sys
+#mn = pyrodigal_manager(file = sys.argv[1])
+#mn.import_sequences()
+#mn.train_manager()
+#mn.predict_genes()
+#mn.translate()
```

### Comparing `RecruitPlotEasy-3.0.9/rpe2_code/supports/sam_parser.py` & `RecruitPlotEasy-3.1.0/rpe2_code/supports/sam_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 		segs = line.strip().split("\t")
 		query = segs[0]
 		
 		#Unaligned read.
 		if query is None or query == "":
 			return None
 		
-		
 		target = segs[2]
 		#Sam is 1-indexed. For python, we want 0.
 		start = int(segs[3]) - 1
 		cig = segs[5]
 		read_len = len(segs[9])
 		covered_ranges = cigar_to_pos(cig, start)
 		covered_ranges.parse_cig_sam()
@@ -43,21 +42,21 @@
 		mdz_seg = mdz_seg[5:]
 		#Get num matches
 		parsed_mds = mdz_to_match_count(mdz_seg)
 		matches, mismatches = parsed_mds.get_match_mismatch()
 		
 		total_align = matches+mismatches
 		
-		pct_id_local = matches / total_align
+		pct_id_local = (matches / total_align) * 100
 		#The second item in the last tuple of covered range is the last pos covered + 1, adjust it back
 		last_pos_aligned = covered_ranges[len(covered_ranges)-1][1] - 1
 		#We don't need to pad the last pos covered
-		pct_id_global = matches / (last_pos_aligned - start)
+		pct_id_global = (matches / read_len) * 100
 		
-		pct_alignment = total_align / read_len
+		pct_alignment = (total_align / read_len) * 100
 		'''
 		as_np_list = []
 		for tuple in covered_ranges:
 			for index in tuple:
 				as_np_list.append(index)
 		covered_ranges = np.array(as_np_list, dtype = np.int32)
 		'''
```

### Comparing `RecruitPlotEasy-3.0.9/setup.py` & `RecruitPlotEasy-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="RecruitPlotEasy",
-	version="3.0.9",
+	version="3.1.0",
 	author="Kenji Gerhardt",
 	author_email="kenji.gerhardt@gmail.com",
 	description="A tool for visualizing short read mapping efforts",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	packages=setuptools.find_packages(),
 	include_package_data=True,
@@ -18,12 +18,12 @@
 		'numpy',
 		'pyrodigal>=2.0',
 		'plotly',
 	],
 	entry_points={
 		"console_scripts": [
 			"rpe=rpe2_code.rpe2_main:main",
-			"recruitploteasy=rpe2_code.rpe2_main:main",
+			"recruitploteasy=rpe2_code.rpe2_main:main"
 		]
 	}
 )
```

