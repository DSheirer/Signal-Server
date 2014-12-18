Signal-Server RF coverage calculator
====================================

/****************************************************************************\
*	   Signal Server: Server optimised SPLAT! by Alex Farrant                *
******************************************************************************
*	SPLAT! Project started in 1997 by John A. Magliacane, KD2BD 	         *
*					                                                         *
******************************************************************************
*         Please consult the SPLAT! documentation for a complete list of     *
*	     individuals who have contributed to this project. 		             *
******************************************************************************
*                                                                            *
*  This program is free software; you can redistribute it and/or modify it   *
*  under the terms of the GNU General Public License as published by the     *
*  Free Software Foundation; either version 2 of the License or any later    *
*  version.								     *
* 									     *
*  This program is distributed in the hope that it will useful, but WITHOUT  *
*  ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or     *
*  FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License     *
*  for more details.							     *
*									     *
******************************************************************************
* g++ -Wall -O3 -s -lm -fomit-frame-pointer itwom3.0.cpp cost.cpp hata.cpp fspl.cpp main.cpp -o ss  * 
\****************************************************************************/

	Usage: signalserver (options)
	
			
                       -d Directory containing .sdf tiles
                     -lat Tx Latitude (decimal degrees)
                     -lon Tx Longitude (decimal degrees) Positive 0-360 
                     -txh Tx Height (above ground), 0 to 60,000 f/m
                       -f Tx Frequency, 20MHz to 100GHz
                     -erp Tx Effective Radiated Power, 0.01 to 5,000,000 Watts
		             -rxh Rx Height(s) (optional. Default=0.1), 0 to 60,000 f/m
                      -rt Rx Threshold (dB / dBm / dBuV/m)
                      -hp Horizontal Polarisation (default=vertical)
		              -gc Ground clutter (feet/meters)
                      -udt User defined terrain filename
	                 -dbm Plot Rxd signal power instead of field strength
	                   -m Metric units of measurement
                      -te Terrain code 1-6 (optional)
                      -terdic Terrain dielectric value 2-80 (optional)
	                  -tercon Terrain conductivity 0.01-0.0001 (optional)
                      -cl Climate code 1-6 (optional)
                       -o Filename. Required. 
                       -R Radius (miles/kilometers)
                     -res Pixels per degree. 300/600/1200(default)/3600 (optional)
                     -t Terrain background
					 -pm Propagation model. 1: ITM (Default), 2: LOS, 3-5: Hata
					 -ked Knife edge diffraction (Default for ITM)
					 -wf Win32 SDF tile names ('=' not ':')
					 -dbg Debug mode