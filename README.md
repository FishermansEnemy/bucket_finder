# == Bucket Finder - Trawl Amazon S3 buckets for interesting files
#
# Each group of files on Amazon S3 have to be contained in a bucket and each bucket has to have a unique
# name across the system. This means that it is possible to bruteforce names, this script does this and more
#
# For more information on how this works see my blog post "Whats in Amazon's buckets?" at
#   http://www.digininja.org/blog/whats_in_amazons_buckets.php
#
# == Version
#
#  1.0 - Released
#  1.1 - Added log to file option
#  1.2 - Added exception handling to the non-download net code [Ian Williams]
#
# == Usage
#
# bucket_finder.rb <wordlist>
#
# -l, --log-file <file name>:
#   filename to log output to
# -d, --download:
#   download any public files found
# -r, --region:
# 	specify the start region
# -h, --help:
#	show help
#
# <wordlist>: the names to brute force
#
# Author:: Robin Wood (robin@digininja.org
# Author:: Ian Williams (ian@fishermansenemy.com) contributor after 1.1
# Copyright:: Copyright (c) Robin Wood 2011
# Licence:: Creative Commons Attribution-Share Alike Licence
#
