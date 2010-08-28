cho  version 1.0.0
Simple text-based command line expenditure record
First option must be a mode specifier:
  -u Update  -d Delete  -s Show
Update: cho -u [date] name price
  Update entry.
  Same entry name is overwritten.
Delete: cho -d [date]
  List entrys , then delete specified entry
Show  : cho -s [option] [date]
  Show statics.
  -v    Verbose (level1)
  -vv   Verbose (level2)
  -vvv  Verbose (level3)
  -V    same as -vv
date example :
  y,m,d is today's date
  8         # y/m/8
  8/1       # y/8/1
  2010/8/1  # 2010/8/1
  2010/8    # 2010/8/*  (Only show mode)
  2010      # 2010/*/*  (Only show mode)
  /         # y/m/*     (Only show mode)
if date is not given, use today's date
data is saved in $CHO_HOME_DIR (default: ~/.cho or ~\cho (win))\
