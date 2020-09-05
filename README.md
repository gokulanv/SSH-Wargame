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

cat data.txt | xxd -r > data
file data
mv data data2.gz
gzip -d data2.gz
file data
file data2
mv data2 data2.bz
bzip2 -d data2.bz
file data2
mv data2 data2.gz
gzip -d data2.gz
file data2
tar -xvf data2
file data5.bin
tar -xvf data5.bin
file data6.bin
mv data6.bin data6.bz
bzip2 -d data6.bz
file data6
tar -xvf data6
file data8.bin
mv data8.bin data8.gz
gzip -d data8.gz
cat data8

>> The password is 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL


## Level 13
ssh bandit.labs.overthewire.org -p 2220 -l bandit13
8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL

ssh -i sshkey.private bandit14@localhost

## Level 14
cat /etc/bandit_pass/bandit14
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e

nc localhost 30000
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e

## Level 15
ssh bandit.labs.overthewire.org -p 2220 -l bandit15
Level 15 Password: BfMYroe26WYalil77FoDi9qh59eK5xNr

echo "BfMYroe26WYalil77FoDi9qh59eK5xNr" | openssl s_client -connect localhost:30001 -ign_eof

## Level 16 
ssh bandit.labs.overthewire.org -p 2220 -l bandit16
cluFn7wTiGryunymYOu4RcffSxQluehd


## WECHALL Credentials
export WECHALLUSER="gvikashb";export WECHALLTOKEN="23D12-4DFF8-8C0D4-18F93-BA4AD-AFC9B";




