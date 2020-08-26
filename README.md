# SSH-Wargame
The Bandit wargame is aimed at learning and using SSH commands.

## Level-0
ssh bandit.labs.overthewire.org -p 2220 -l bandit0
Password: bandit0

cat readme // to get password for level 1
exit

## Level-1
ssh bandit.labs.overthewire.org -p 2220 -l bandit1
Password: boJ9jbbUNNfktd78OOpsqOltutMc3MY1

cat ./-
exit

## Level 2
ssh bandit.labs.overthewire.org -p 2220 -l bandit2
Password: CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9

cat "spaces in this filename"
exit

## Level 3
ssh bandit.labs.overthewire.org -p 2220 -l bandit3
UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

cd inhere
ls -a
cat .hidden

## Level 4
ssh bandit.labs.overthewire.org -p 2220 -l bandit4
pIwrPrtPN36QITSp3EQaw936yaFoFgAB

file ./* | grep ASCII | cut -c1-9 | cut -c1-9 | xargs -0 -d '\n' cat

## Level 5
ssh bandit.labs.overthewire.org -p 2220 -l bandit5

find . -type f -size 1033c ! -executable -exec file {} + | grep ASCII | cut -d':' -f 1 | xargs -0 -d '\n' cat

## Level 6
ssh bandit.labs.overthewire.org -p 2220 -l bandit6
DXjZPULLxYr17uwoI01bNLQbtFemEgo7

find . -size 33c -user bandit7 -group bandit6 2>/dev/null | xargs -0 -d '\n' cat

## Level 7
ssh bandit.labs.overthewire.org -p 2220 -l bandit7
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

cat data.txt | grep millionth | cut -f2

## Level 8
ssh bandit.labs.overthewire.org -p 2220 -l bandit8
cvX2JJa4CFALtqS87jk27qwqGhBM9plV

sort data.txt | uniq -u

## Level 9
ssh bandit.labs.overthewire.org -p 2220 -l bandit9
UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR

 strings -f data.txt | grep -E '(=)\1{2,}'

## Level 10
ssh bandit.labs.overthewire.org -p 2220 -l bandit10
truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk

cat data.txt | base64 decode

## Level 11
ssh bandit.labs.overthewire.org -p 2220 -l bandit11
IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR

cat data.txt | tr '[a-zA-Z]' '[n-za-mN-ZA-M]' 

## Level 12
ssh bandit.labs.overthewire.org -p 2220 -l bandit12
5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu




















