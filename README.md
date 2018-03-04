# Snort Log enhancer 

This Tool enhances your default snort logfile's with geoip informationen.
For more information take a look at the example section.

## Build binaries
- Cd into the blocklog folder
```
cd src/blocklog 
```
- Resolve packages
```
go get
```
- Build the executable
```
go install
```

## How to use
You can find the executable in the bin subfolder of the project root folder

- Start BlockLog (Linux)
```
./blocklog 
```
- Follow the displayed instructions - Info : The logfile should be in the same folder as the executable
- The final csv will be outputted in the same directory and is named block_log_enhanced.csv 

## Example
#### BlockLog
- The default snort IP Blocklist logfile looks like this:
```
1.2.3.4
5.6.7.8
```
- BlockLog will create an enhanced version of the logfile, which will look like this: 
```
1.2.3.4,United States
5.6.7.8,Germany
```

