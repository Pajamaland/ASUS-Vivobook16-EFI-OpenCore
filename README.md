# ASUS Vivobook 16 M1605Y (Ryzen 7 7730U) - OpenCore EFI - macOS 13 Ventura
![MacVivobook](/assets/images/macvivobook.png)
### HEAVY WORK IN PROGRESS. 
I'm not *actively* working on this (ie, I have a life), but open an issue if you have any problems and I may spend a bit of time troubleshooting to see if I/we can solve it. I make no guarantee of future updates or updating the EFI to support newer macOS versions (although it *might* work with Sonoma. Does NOT work with Seqouia.)

## Specifications
Ryzen 7 7730U (with Vega graphics)  
24GB RAM (8GB soldered, 16GB SODIMM)  
Crucial P2 1TB NVMe SSD  

## Issues
- Sleep will not work, *ever*. This is due to the fact that the laptop doesn't support S3, only S0ix.  
  You can bypass this by just using hibernation. (``sudo pmset -a hibernatemode 25``) On an SSD, the wake time isn't too bad.  
- Hardware acceleration for Chromium-based applications & Firefox not working (will crash immediately).  
- Can't use Fn lock.  
  
Everything else works fine as far as I can tell.
