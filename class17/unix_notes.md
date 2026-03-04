## Core Unix Commands 

Most unix commands have short names, which makes them quick to type but annoying to learn.

pwd:    Print working directory
ls:     List files and directories
cd:     Change directory
mkdir:  Make a new directory
rm:     Remove files and directories (delete)
cp:     Copy files and directories (source > destination)
mv:     Moves files or directories (rename)
nano:   A text editor (very basic, but always available)

curl:   Download files from the web or ftp
wget:   Download files from the web
tar -zxvf: UnTar (unpackage) Tar archive files
gunzip: UnZip files
$PATH:  The places (directories) to look for programs

## AWS EC2 Instance

ssh to join
scp for secure copy

## Class 17

ssh -i ~/Downloads/bioinf_aadhyat.pem ubuntu@ec2-34-209-250-157.us-west-2.compute.amazonaws.com

Make it easier to access AWS server (type the following into the console):

export KEY=~/Downloads/bioinf_aadhyat.pem
export SERVER=ubuntu@ec2-34-209-250-157.us-west-2.compute.amazonaws.com

Then we can use:

ssh -i $KEY $SERVER

scp -r -i $KEY $SERVER:~/*_quant .