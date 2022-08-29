Here's the breakdown:

$P = Current Directory's Path
$_ = Carriage Return
$+ = A plus sign for each level in the PUSHD/POPD stack.
Here's some other interesting prompts. Paste these into any CMD.EXE window:

set prompt=[%computername%] $d$s$t$_$p$_$_$+$g

yields this. Note the use of an environment variables within a prompt. Here's an extensive list of environment variables.

[SCOTTPC] Thu 07/13/2006 22:19:20.40
C:\Documents and Settings\Scott

Another nice one:

set=prompt=$m$_$p$g

yields this when on a UNC Mapped Drive:

\\FREDPC\C$
Z:\Documents and Settings\Fred

There's all sorts of crap that PROMPT /? gives you:

  $A   & (Ampersand)
  $B   | (pipe)
  $C   ( (Left parenthesis)
  $D   Current date
  $E   Escape code (ASCII code 27)
  $F   ) (Right parenthesis)
  $G   > (greater-than sign)
  $H   Backspace (erases previous character)
  $L   < (less-than sign)
  $N   Current drive
  $P   Current drive and path
  $Q   = (equal sign)
  $S     (space)
  $T   Current time
  $V   Windows XP version number
  $_   Carriage return and linefeed
  $$   $ (dollar sign)
  $+   zero or more plus sign (+) characters depending upon the
       depth of the PUSHD directory stack, one character for each
       level pushed.
  $M   Displays the remote name associated with the current drive
       letter or the empty string if current drive is not a network
       drive.




# set to default prompt:
```$ set PROMPT=$P$G```


The CMD prompt can be edited adding/editing the PROMPT variable in 'system variables'. 


It can also be change directly via CMD by typing the following command. 
```$ set PROMPT=$P$G```		# this is the default prompt that comes with Windows.


Commands:
SETX - Set an environment variable permanently.
