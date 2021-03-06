# MLAG Config Check

## Description
This Python script checks to ensure that all VLANs on MLAG ports are also present on the ISC.

If any VLANs are missing from the ISC, the script will output the VLAN name and the MLAG port that is added to the VLAN.

### Files
* [mlag_config_check.py](mlag_config_check.py)
* [README.md](README.md)

### Requirements
* Firmware: ExtremeXOS(TM) 15.6+
* Platform(s): Any ExtremeXOS switch

### Example

Correct MLAG configuration:
```
mlag1.3 # run script mlag_config_check.py
MLAG config check completed.
```

Incorrect MLAG configuration:
```
mlag1.7 # run script mlag_config_check.py
Vlan problem is not added to the ISC port (1), and is found on MLAG port 3. Please correct.
MLAG config check completed.
```

## Notes
This currently only supports MLAG implementations with one MLAG peer.

## License
Copyright© 2015, Extreme Networks.  All rights reserved.

Redistribution and use in source and binary forms, with or without modification,
are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this
list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice,
this list of conditions and the following disclaimer in the documentation
and/or other materials provided with the distribution.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

## Support
The software is provided as is and Extreme Networks has no obligation to provide
maintenance, support, updates, enhancements or modifications.
Any support provided by Extreme Networks is at its sole discretion.

Issues and/or bug fixes may be reported on [The Hub](https://community.extremenetworks.com/extreme).

>Be Extreme
