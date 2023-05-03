# Comparing `tmp/parsedmarc-8.4.2.tar.gz` & `tmp/parsedmarc-8.5.0.tar.gz`

## Comparing `parsedmarc-8.4.2.tar` & `parsedmarc-8.5.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0    61120 2020-02-02 00:00:00.000000 parsedmarc-8.4.2/parsedmarc/__init__.py
--rw-r--r--   0        0        0    46812 2020-02-02 00:00:00.000000 parsedmarc-8.4.2/parsedmarc/cli.py
--rw-r--r--   0        0        0    20853 2020-02-02 00:00:00.000000 parsedmarc-8.4.2/parsedmarc/elastic.py
--rw-r--r--   0        0        0     6160 2020-02-02 00:00:00.000000 parsedmarc-8.4.2/parsedmarc/kafkaclient.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 parsedmarc-8.4.2/parsedmarc/log.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 parsedmarc-8.4.2/parsedmarc/s3.py
--rw-r--r--   0        0        0     6157 2020-02-02 00:00:00.000000 parsedmarc-8.4.2/parsedmarc/splunk.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 parsedmarc-8.4.2/parsedmarc/syslog.py
--rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 parsedmarc-8.4.2/parsedmarc/utils.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 parsedmarc-8.4.2/parsedmarc/mail/__init__.py
--rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 parsedmarc-8.4.2/parsedmarc/mail/gmail.py
--rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 parsedmarc-8.4.2/parsedmarc/mail/graph.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 parsedmarc-8.4.2/parsedmarc/mail/imap.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 parsedmarc-8.4.2/parsedmarc/mail/mailbox_connection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsedmarc-8.4.2/parsedmarc/resources/__init__.py
--rwxr-xr-x   0        0        0  7028733 2020-02-02 00:00:00.000000 parsedmarc-8.4.2/parsedmarc/resources/dbip-country-lite.mmdb
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 parsedmarc-8.4.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 parsedmarc-8.4.2/LICENSE
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 parsedmarc-8.4.2/README.md
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 parsedmarc-8.4.2/pyproject.toml
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 parsedmarc-8.4.2/PKG-INFO
+-rw-r--r--   0        0        0    61170 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/__init__.py
+-rw-r--r--   0        0        0    48948 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/cli.py
+-rw-r--r--   0        0        0    20853 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/elastic.py
+-rw-r--r--   0        0        0     6160 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/kafkaclient.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/log.py
+-rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/loganalytics.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/s3.py
+-rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/splunk.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/syslog.py
+-rw-r--r--   0        0        0    17841 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/utils.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/mail/__init__.py
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/mail/gmail.py
+-rw-r--r--   0        0        0    10005 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/mail/graph.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/mail/imap.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/mail/mailbox_connection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/resources/__init__.py
+-rwxr-xr-x   0        0        0  7028733 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/resources/dbip-country-lite.mmdb
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/LICENSE
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/README.md
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/PKG-INFO
```

### Comparing `parsedmarc-8.4.2/parsedmarc/__init__.py` & `parsedmarc-8.5.0/parsedmarc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from parsedmarc.log import logger
 from parsedmarc.mail import MailboxConnection
 from parsedmarc.utils import get_base_domain, get_ip_address_info
 from parsedmarc.utils import is_outlook_msg, convert_outlook_msg
 from parsedmarc.utils import parse_email
 from parsedmarc.utils import timestamp_to_human, human_timestamp_to_datetime
 
-__version__ = "8.4.2"
+__version__ = "8.5.0"
 
 logger.debug("parsedmarc v{0}".format(__version__))
 
 feedback_report_regex = re.compile(r"^([\w\-]+): (.+)$", re.MULTILINE)
 xml_header_regex = re.compile(r"^<\?xml .*?>", re.MULTILINE)
 xml_schema_regex = re.compile(r"</??xs:schema.*>", re.MULTILINE)
 text_report_regex = re.compile(r"\s*([a-zA-Z\s]+):\s(.+)", re.MULTILINE)
@@ -204,15 +204,15 @@
     """Parses a DMARC XML report string and returns a consistent OrderedDict
 
     Args:
         xml (str): A string of DMARC aggregate report XML
         ip_db_path (str): Path to a MMDB file from MaxMind or DBIP
         offline (bool): Do not query online for geolocation or DNS
         nameservers (list): A list of one or more nameservers to use
-        (Cloudflare's public DNS resolvers by default)
+            (Cloudflare's public DNS resolvers by default)
         timeout (float): Sets the DNS timeout in seconds
         parallel (bool): Parallel processing
         keep_alive (callable): Keep alive function
 
     Returns:
         OrderedDict: The parsed aggregate DMARC report
     """
@@ -405,15 +405,15 @@
     aggregate DMARC report
 
     Args:
         _input: A path to a file, a file like object, or bytes
         offline (bool): Do not query online for geolocation or DNS
         ip_db_path (str): Path to a MMDB file from MaxMind or DBIP
         nameservers (list): A list of one or more nameservers to use
-        (Cloudflare's public DNS resolvers by default)
+            (Cloudflare's public DNS resolvers by default)
         dns_timeout (float): Sets the DNS timeout in seconds
         parallel (bool): Parallel processing
         keep_alive (callable): Keep alive function
 
     Returns:
         OrderedDict: The parsed DMARC aggregate report
     """
@@ -578,18 +578,18 @@
     Args:
         feedback_report (str): A message's feedback report as a string
         ip_db_path (str): Path to a MMDB file from MaxMind or DBIP
         offline (bool): Do not query online for geolocation or DNS
         sample (str): The RFC 822 headers or RFC 822 message sample
         msg_date (str): The message's date header
         nameservers (list): A list of one or more nameservers to use
-        (Cloudflare's public DNS resolvers by default)
+            (Cloudflare's public DNS resolvers by default)
         dns_timeout (float): Sets the DNS timeout in seconds
         strip_attachment_payloads (bool): Remove attachment payloads from
-        forensic report results
+            forensic report results
         parallel (bool): Parallel processing
 
     Returns:
         OrderedDict: A parsed report and sample
     """
     delivery_results = ["delivered", "spam", "policy", "reject", "other"]
 
@@ -768,15 +768,15 @@
     Args:
         input_: An emailed DMARC report in RFC 822 format, as bytes or a string
         ip_db_path (str): Path to a MMDB file from MaxMind or DBIP
         offline (bool): Do not query online for geolocation on DNS
         nameservers (list): A list of one or more nameservers to use
         dns_timeout (float): Sets the DNS timeout in seconds
         strip_attachment_payloads (bool): Remove attachment payloads from
-        forensic report results
+            forensic report results
         parallel (bool): Parallel processing
         keep_alive (callable): keep alive function
 
     Returns:
         OrderedDict:
         * ``report_type``: ``aggregate`` or ``forensic``
         * ``report``: The parsed report
@@ -910,18 +910,18 @@
                       offline=False, parallel=False, keep_alive=None):
     """Parses a DMARC aggregate or forensic file at the given path, a
     file-like object. or bytes
 
     Args:
         input_: A path to a file, a file like object, or bytes
         nameservers (list): A list of one or more nameservers to use
-        (Cloudflare's public DNS resolvers by default)
+            (Cloudflare's public DNS resolvers by default)
         dns_timeout (float): Sets the DNS timeout in seconds
         strip_attachment_payloads (bool): Remove attachment payloads from
-        forensic report results
+            forensic report results
         ip_db_path (str): Path to a MMDB file from MaxMind or DBIP
         offline (bool): Do not make online queries for geolocation or DNS
         parallel (bool): Parallel processing
         keep_alive (callable): Keep alive function
 
     Returns:
         OrderedDict: The parsed DMARC report
@@ -970,24 +970,24 @@
                                 parallel=False):
     """Parses a mailbox in mbox format containing e-mails with attached
     DMARC reports
 
     Args:
         input_: A path to a mbox file
         nameservers (list): A list of one or more nameservers to use
-        (Cloudflare's public DNS resolvers by default)
+            (Cloudflare's public DNS resolvers by default)
         dns_timeout (float): Sets the DNS timeout in seconds
         strip_attachment_payloads (bool): Remove attachment payloads from
-        forensic report results
+            forensic report results
         ip_db_path (str): Path to a MMDB file from MaxMind or DBIP
         offline (bool): Do not make online queries for geolocation or DNS
         parallel (bool): Parallel processing
 
     Returns:
-        OrderedDict: Lists of  ``aggregate_reports`` and ``forensic_reports``
+        OrderedDict: Lists of ``aggregate_reports`` and ``forensic_reports``
 
     """
     aggregate_reports = []
     forensic_reports = []
     try:
         mbox = mailbox.mbox(input_)
         message_keys = mbox.keys()
@@ -1044,20 +1044,20 @@
         delete (bool): Delete  messages after processing them
         test (bool): Do not move or delete messages after processing them
         ip_db_path (str): Path to a MMDB file from MaxMind or DBIP
         offline (bool): Do not query online for geolocation or DNS
         nameservers (list): A list of DNS nameservers to query
         dns_timeout (float): Set the DNS query timeout
         strip_attachment_payloads (bool): Remove attachment payloads from
-          forensic report results
+            forensic report results
         results (dict): Results from the previous run
         batch_size (int): Number of messages to read and process before saving
             (use 0 for no limit)
         create_folders (bool): Whether to create the destination folders
-          (not used in watch)
+            (not used in watch)
 
     Returns:
         OrderedDict: Lists of ``aggregate_reports`` and ``forensic_reports``
     """
     if delete and test:
         raise ValueError("delete and test options are mutually exclusive")
 
@@ -1226,22 +1226,22 @@
         mailbox_connection: The mailbox connection object
         callback: The callback function to receive the parsing results
         reports_folder: The IMAP folder where reports can be found
         archive_folder: The folder to move processed mail to
         delete (bool): Delete  messages after processing them
         test (bool): Do not move or delete messages after processing them
         check_timeout (int): Number of seconds to wait for a IMAP IDLE response
-          or the number of seconds until the next mail check
+            or the number of seconds until the next mail check
         ip_db_path (str): Path to a MMDB file from MaxMind or DBIP
         offline (bool): Do not query online for geolocation or DNS
         nameservers (list): A list of one or more nameservers to use
-        (Cloudflare's public DNS resolvers by default)
+            (Cloudflare's public DNS resolvers by default)
         dns_timeout (float): Set the DNS query timeout
         strip_attachment_payloads (bool): Replace attachment payloads in
-        forensic report samples with None
+            forensic report samples with None
         batch_size (int): Number of messages to read and process before saving
     """
 
     def check_callback(connection):
         sa = strip_attachment_payloads
         res = get_dmarc_reports_from_mailbox(connection=connection,
                                              reports_folder=reports_folder,
@@ -1421,15 +1421,15 @@
         port (int): Port to use
         require_encryption (bool): Require a secure connection from the start
         verify (bool): verify the SSL/TLS certificate
         username (str): An optional username
         password (str): An optional password
         subject (str): Overrides the default message subject
         attachment_filename (str): Override the default attachment filename
-        message (str: Override the default plain text body
+        message (str): Override the default plain text body
     """
     logger.debug("Emailing report to: {0}".format(",".join(mail_to)))
     date_string = datetime.now().strftime("%Y-%m-%d")
     if attachment_filename:
         if not attachment_filename.lower().endswith(".zip"):
             attachment_filename += ".zip"
         filename = attachment_filename
```

### Comparing `parsedmarc-8.4.2/parsedmarc/cli.py` & `parsedmarc-8.5.0/parsedmarc/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import sys
 import time
 from tqdm import tqdm
 
 from parsedmarc import get_dmarc_reports_from_mailbox, watch_inbox, \
     parse_report_file, get_dmarc_reports_from_mbox, elastic, kafkaclient, \
     splunk, save_output, email_results, ParserError, __version__, \
-    InvalidDMARCReport, s3, syslog
+    InvalidDMARCReport, s3, syslog, loganalytics
 
 from parsedmarc.mail import IMAPConnection, MSGraphConnection, GmailConnection
 from parsedmarc.mail.graph import AuthMethod
 
 from parsedmarc.log import logger
 from parsedmarc.utils import is_mbox
 
@@ -166,14 +166,37 @@
                 try:
                     forensic_reports_ = reports_["forensic_reports"]
                     if len(forensic_reports_) > 0:
                         hec_client.save_forensic_reports_to_splunk(
                             forensic_reports_)
                 except splunk.SplunkError as e:
                     logger.error("Splunk HEC error: {0}".format(e.__str__()))
+        if opts.la_dce:
+            try:
+                la_client = loganalytics.LogAnalyticsClient(
+                    client_id=opts.la_client_id,
+                    client_secret=opts.la_client_secret,
+                    tenant_id=opts.la_tenant_id,
+                    dce=opts.la_dce,
+                    dcr_immutable_id=opts.la_dcr_immutable_id,
+                    dcr_aggregate_stream=opts.la_dcr_aggregate_stream,
+                    dcr_forensic_stream=opts.la_dcr_forensic_stream
+                )
+                la_client.publish_results(
+                    reports_,
+                    opts.save_aggregate,
+                    opts.save_forensic)
+            except loganalytics.LogAnalyticsException as e:
+                logger.error("Log Analytics error: {0}".format(e.__str__()))
+            except Exception as e:
+                logger.error(
+                    "Unknown error occured" +
+                    " during the publishing" +
+                    " to Log Analitics: " +
+                    e.__str__())
 
     arg_parser = ArgumentParser(description="Parses DMARC reports")
     arg_parser.add_argument("-c", "--config-file",
                             help="a path to a configuration file "
                                  "(--silent implied)")
     arg_parser.add_argument("file_path", nargs="*",
                             help="one or more paths to aggregate or forensic "
@@ -309,15 +332,22 @@
                      gmail_api_token_file=None,
                      gmail_api_include_spam_trash=False,
                      gmail_api_scopes=[],
                      gmail_api_oauth2_port=8080,
                      log_file=args.log_file,
                      n_procs=1,
                      chunk_size=1,
-                     ip_db_path=None
+                     ip_db_path=None,
+                     la_client_id=None,
+                     la_client_secret=None,
+                     la_tenant_id=None,
+                     la_dce=None,
+                     la_dcr_immutable_id=None,
+                     la_dcr_aggregate_stream=None,
+                     la_dcr_forensic_stream=None
                      )
     args = arg_parser.parse_args()
 
     if args.config_file:
         abs_path = os.path.abspath(args.config_file)
         if not os.path.exists(abs_path):
             logger.error("A file does not exist at {0}".format(abs_path))
@@ -717,14 +747,30 @@
                 gmail_api_config.get("scopes",
                                      default_gmail_api_scope)
             opts.gmail_api_scopes = \
                 _str_to_list(opts.gmail_api_scopes)
             if "oauth2_port" in gmail_api_config:
                 opts.gmail_api_oauth2_port = \
                     gmail_api_config.get("oauth2_port", 8080)
+        if "log_analytics" in config.sections():
+            log_analytics_config = config["log_analytics"]
+            opts.la_client_id = \
+                log_analytics_config.get("client_id")
+            opts.la_client_secret = \
+                log_analytics_config.get("client_secret")
+            opts.la_tenant_id = \
+                log_analytics_config.get("tenant_id")
+            opts.la_dce = \
+                log_analytics_config.get("dce")
+            opts.la_dcr_immutable_id = \
+                log_analytics_config.get("dcr_immutable_id")
+            opts.la_dcr_aggregate_stream = \
+                log_analytics_config.get("dcr_aggregate_stream")
+            opts.la_dcr_forensic_stream = \
+                log_analytics_config.get("dcr_forensic_stream")
 
     logger.setLevel(logging.ERROR)
 
     if opts.warnings:
         logger.setLevel(logging.WARNING)
     if opts.verbose:
         logger.setLevel(logging.INFO)
```

### Comparing `parsedmarc-8.4.2/parsedmarc/elastic.py` & `parsedmarc-8.5.0/parsedmarc/elastic.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.4.2/parsedmarc/kafkaclient.py` & `parsedmarc-8.5.0/parsedmarc/kafkaclient.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.4.2/parsedmarc/s3.py` & `parsedmarc-8.5.0/parsedmarc/s3.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.4.2/parsedmarc/splunk.py` & `parsedmarc-8.5.0/parsedmarc/splunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,22 +22,23 @@
     # http://docs.splunk.com/Documentation/Splunk/latest/Data/AboutHEC
     # http://docs.splunk.com/Documentation/Splunk/latest/RESTREF/RESTinput#services.2Fcollector
 
     def __init__(self, url, access_token, index,
                  source="parsedmarc", verify=True, timeout=60):
         """
         Initializes the HECClient
+
         Args:
             url (str): The URL of the HEC
             access_token (str): The HEC access token
             index (str): The name of the index
             source (str): The source name
             verify (bool): Verify SSL certificates
             timeout (float): Number of seconds to wait for the server to send
-            data before giving up
+                data before giving up
         """
         url = urlparse(url)
         self.url = "{0}://{1}/services/collector/event/1.0".format(url.scheme,
                                                                    url.netloc)
         self.access_token = access_token.lstrip("Splunk ")
         self.index = index
         self.host = socket.getfqdn()
@@ -55,15 +56,15 @@
 
     def save_aggregate_reports_to_splunk(self, aggregate_reports):
         """
         Saves aggregate DMARC reports to Splunk
 
         Args:
             aggregate_reports: A list of aggregate report dictionaries
-            to save in Splunk
+                to save in Splunk
 
         """
         logger.debug("Saving aggregate reports to Splunk")
         if type(aggregate_reports) == dict:
             aggregate_reports = [aggregate_reports]
 
         if len(aggregate_reports) < 1:
@@ -121,16 +122,16 @@
             raise SplunkError(response["text"])
 
     def save_forensic_reports_to_splunk(self, forensic_reports):
         """
         Saves forensic DMARC reports to Splunk
 
         Args:
-            forensic_reports (list):  A list of forensic report dictionaries
-            to save in Splunk
+            forensic_reports (list): A list of forensic report dictionaries
+                to save in Splunk
         """
         logger.debug("Saving forensic reports to Splunk")
         if type(forensic_reports) == dict:
             forensic_reports = [forensic_reports]
 
         if len(forensic_reports) < 1:
             return
```

### Comparing `parsedmarc-8.4.2/parsedmarc/syslog.py` & `parsedmarc-8.5.0/parsedmarc/syslog.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.4.2/parsedmarc/utils.py` & `parsedmarc-8.5.0/parsedmarc/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     Queries DNS
 
     Args:
         domain (str): The domain or subdomain to query about
         record_type (str): The record type to query for
         cache (ExpiringDict): Cache storage
         nameservers (list): A list of one or more nameservers to use
-        (Cloudflare's public DNS resolvers by default)
+            (Cloudflare's public DNS resolvers by default)
         timeout (float): Sets the DNS timeout in seconds
 
     Returns:
         list: A list of answers
     """
     domain = str(domain).lower()
     record_type = record_type.upper()
@@ -184,15 +184,15 @@
     """
     Resolves an IP address to a hostname using a reverse DNS query
 
     Args:
         ip_address (str): The IP address to resolve
         cache (ExpiringDict): Cache storage
         nameservers (list): A list of one or more nameservers to use
-        (Cloudflare's public DNS resolvers by default)
+            (Cloudflare's public DNS resolvers by default)
         timeout (float): Sets the DNS query timeout in seconds
 
     Returns:
         str: The reverse DNS hostname (if any)
     """
     hostname = None
     try:
@@ -205,21 +205,21 @@
         pass
 
     return hostname
 
 
 def timestamp_to_datetime(timestamp):
     """
-    Converts a UNIX/DMARC timestamp to a Python ``DateTime`` object
+    Converts a UNIX/DMARC timestamp to a Python ``datetime`` object
 
     Args:
         timestamp (int): The timestamp
 
     Returns:
-        DateTime: The converted timestamp as a Python ``DateTime`` object
+        datetime: The converted timestamp as a Python ``datetime`` object
     """
     return datetime.fromtimestamp(int(timestamp))
 
 
 def timestamp_to_human(timestamp):
     """
     Converts a UNIX/DMARC timestamp to a human-readable string
@@ -231,22 +231,22 @@
         str: The converted timestamp in ``YYYY-MM-DD HH:MM:SS`` format
     """
     return timestamp_to_datetime(timestamp).strftime("%Y-%m-%d %H:%M:%S")
 
 
 def human_timestamp_to_datetime(human_timestamp, to_utc=False):
     """
-    Converts a human-readable timestamp into a Python ``DateTime`` object
+    Converts a human-readable timestamp into a Python ``datetime`` object
 
     Args:
         human_timestamp (str): A timestamp string
         to_utc (bool): Convert the timestamp to UTC
 
     Returns:
-        DateTime: The converted timestamp
+        datetime: The converted timestamp
     """
 
     human_timestamp = human_timestamp.replace("-0000", "")
     human_timestamp = parenthesis_regex.sub("", human_timestamp)
 
     dt = parse_date(human_timestamp)
     return dt.astimezone(timezone.utc) if to_utc else dt
@@ -334,15 +334,15 @@
 
     Args:
         ip_address (str): The IP address to check
         ip_db_path (str): path to a MMDB file from MaxMind or DBIP
         cache (ExpiringDict): Cache storage
         offline (bool): Do not make online queries for geolocation or DNS
         nameservers (list): A list of one or more nameservers to use
-        (Cloudflare's public DNS resolvers by default)
+            (Cloudflare's public DNS resolvers by default)
         timeout (float): Sets the DNS timeout in seconds
         parallel (bool): parallel processing
 
     Returns:
         OrderedDict: ``ip_address``, ``reverse_dns``
 
     """
@@ -388,14 +388,15 @@
                         ("local", local),
                         ("domain", domain)])
 
 
 def get_filename_safe_string(string):
     """
     Converts a string to a string that is safe for a filename
+
     Args:
         string (str): A string to make safe for a filename
 
     Returns:
         str: A string safe for a filename
     """
     invalid_filename_chars = ['\\', '/', ':', '"', '*', '?', '|', '\n',
@@ -409,42 +410,42 @@
     string = (string[:100]) if len(string) > 100 else string
 
     return string
 
 
 def is_mbox(path):
     """
-    Checks if the given content is a MBOX mailbox file
+    Checks if the given content is an MBOX mailbox file
 
     Args:
         path: Content to check
 
     Returns:
-        bool: A flag the indicates if a file is a MBOX mailbox file
+        bool: A flag that indicates if the file is an MBOX mailbox file
     """
     _is_mbox = False
     try:
         mbox = mailbox.mbox(path)
         if len(mbox.keys()) > 0:
             _is_mbox = True
     except Exception as e:
         logger.debug("Error checking for MBOX file: {0}".format(e.__str__()))
 
     return _is_mbox
 
 
 def is_outlook_msg(content):
     """
-    Checks if the given content is a Outlook msg OLE file
+    Checks if the given content is an Outlook msg OLE/MSG file
 
     Args:
         content: Content to check
 
     Returns:
-        bool: A flag the indicates if a file is a Outlook MSG file
+        bool: A flag that indicates if the file is an Outlook MSG file
     """
     return type(content) == bytes and content.startswith(
         b"\xD0\xCF\x11\xE0\xA1\xB1\x1A\xE1")
 
 
 def convert_outlook_msg(msg_bytes):
     """
@@ -484,15 +485,16 @@
     """
     A simplified email parser
 
     Args:
         data: The RFC 822 message string, or MSG binary
         strip_attachment_payloads (bool): Remove attachment payloads
 
-    Returns (dict): Parsed email data
+    Returns:
+        dict: Parsed email data
     """
 
     if type(data) == bytes:
         if is_outlook_msg(data):
             data = convert_outlook_msg(data)
         data = data.decode("utf-8", errors="replace")
     parsed_email = mailparser.parse_from_string(data)
```

### Comparing `parsedmarc-8.4.2/parsedmarc/mail/gmail.py` & `parsedmarc-8.5.0/parsedmarc/mail/gmail.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.4.2/parsedmarc/mail/graph.py` & `parsedmarc-8.5.0/parsedmarc/mail/graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -141,25 +141,42 @@
                            f'{resp.status_code} {resp.json()}')
 
     def fetch_messages(self, folder_name: str, **kwargs) -> List[str]:
         """ Returns a list of message UIDs in the specified folder """
         folder_id = self._find_folder_id_from_folder_path(folder_name)
         url = f'/users/{self.mailbox_name}/mailFolders/' \
               f'{folder_id}/messages'
+        batch_size = kwargs.get('batch_size')
+        if not batch_size:
+            batch_size = 0
+        emails = self._get_all_messages(url, batch_size)
+        return [email['id'] for email in emails]
+
+    def _get_all_messages(self, url, batch_size):
+        messages: list
         params = {
             '$select': 'id'
         }
-        batch_size = kwargs.get('batch_size')
         if batch_size and batch_size > 0:
             params['$top'] = batch_size
+        else:
+            params['$top'] = 100
         result = self._client.get(url, params=params)
         if result.status_code != 200:
             raise RuntimeError(f'Failed to fetch messages {result.text}')
-        emails = result.json()['value']
-        return [email['id'] for email in emails]
+        messages = result.json()['value']
+        # Loop if next page is present and not obtained message limit.
+        while '@odata.nextLink' in result.json() and (
+                batch_size == 0 or
+                batch_size - len(messages) > 0):
+            result = self._client.get(result.json()['@odata.nextLink'])
+            if result.status_code != 200:
+                raise RuntimeError(f'Failed to fetch messages {result.text}')
+            messages.extend(result.json()['value'])
+        return messages
 
     def mark_message_read(self, message_id: str):
         """Marks a message as read"""
         url = f'/users/{self.mailbox_name}/messages/{message_id}'
         resp = self._client.patch(url, json={"isRead": "true"})
         if resp.status_code != 200:
             raise RuntimeWarning(f"Failed to mark message read"
@@ -219,18 +236,19 @@
     def _find_folder_id_with_parent(self,
                                     folder_name: str,
                                     parent_folder_id: Optional[str]):
         sub_url = ''
         if parent_folder_id is not None:
             sub_url = f'/{parent_folder_id}/childFolders'
         url = f'/users/{self.mailbox_name}/mailFolders{sub_url}'
-        folders_resp = self._client.get(url)
+        filter = f"?$filter=displayName eq '{folder_name}'"
+        folders_resp = self._client.get(url + filter)
         if folders_resp.status_code != 200:
             raise RuntimeWarning(f"Failed to list folders."
                                  f"{folders_resp.json()}")
-        folders = folders_resp.json()['value']
+        folders: list = folders_resp.json()['value']
         matched_folders = [folder for folder in folders
                            if folder['displayName'] == folder_name]
         if len(matched_folders) == 0:
             raise RuntimeError(f"folder {folder_name} not found")
         selected_folder = matched_folders[0]
         return selected_folder['id']
```

### Comparing `parsedmarc-8.4.2/parsedmarc/mail/imap.py` & `parsedmarc-8.5.0/parsedmarc/mail/imap.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.4.2/parsedmarc/mail/mailbox_connection.py` & `parsedmarc-8.5.0/parsedmarc/mail/mailbox_connection.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.4.2/parsedmarc/resources/dbip-country-lite.mmdb` & `parsedmarc-8.5.0/parsedmarc/resources/dbip-country-lite.mmdb`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.4.2/.gitignore` & `parsedmarc-8.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.4.2/LICENSE` & `parsedmarc-8.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.4.2/README.md` & `parsedmarc-8.5.0/README.md`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.4.2/pyproject.toml` & `parsedmarc-8.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     "Intended Audience :: Information Technology",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3"
 ]
 dependencies = [
     "azure-identity>=1.8.0",
+    "azure-monitor-ingestion>=1.0.0",
     "boto3>=1.16.63",
     "dateparser>=1.1.1",
     "dnspython>=2.0.0",
     "elasticsearch-dsl==7.4.0",
     "elasticsearch<7.14.0",
     "expiringdict>=1.1.4",
     "geoip2>=3.0.0",
```

### Comparing `parsedmarc-8.4.2/PKG-INFO` & `parsedmarc-8.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: parsedmarc
-Version: 8.4.2
+Version: 8.5.0
 Summary: A Python package and CLI for parsing aggregate and forensic DMARC reports
 Project-URL: Homepage, https://domainaware.github.io/parsedmarc
 Author-email: Sean Whalen <whalenster@gmail.com>
+License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: DMARC,parser,reporting
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: azure-identity>=1.8.0
+Requires-Dist: azure-monitor-ingestion>=1.0.0
 Requires-Dist: boto3>=1.16.63
 Requires-Dist: dateparser>=1.1.1
 Requires-Dist: dnspython>=2.0.0
 Requires-Dist: elasticsearch-dsl==7.4.0
 Requires-Dist: elasticsearch<7.14.0
 Requires-Dist: expiringdict>=1.1.4
 Requires-Dist: geoip2>=3.0.0
```

