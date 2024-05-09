# Comparing `tmp/pymakeplots-0.1.7.tar.gz` & `tmp/pymakeplots-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymakeplots-0.1.7.tar", last modified: Thu Jun 22 09:35:05 2023, max compression
+gzip compressed data, was "pymakeplots-0.2.0.tar", last modified: Thu May  9 16:29:32 2024, max compression
```

## Comparing `pymakeplots-0.1.7.tar` & `pymakeplots-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-06-22 09:35:05.581225 pymakeplots-0.1.7/
--rw-r--r--   0 tdavis     (501) staff       (20)     1077 2020-09-02 10:40:49.000000 pymakeplots-0.1.7/LICENSE.md
--rw-r--r--   0 tdavis     (501) staff       (20)     1664 2023-06-22 09:35:05.581051 pymakeplots-0.1.7/PKG-INFO
--rwxr-xr-x   0 tdavis     (501) staff       (20)     1225 2020-09-04 16:00:00.000000 pymakeplots-0.1.7/README.md
-drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-06-22 09:35:05.579921 pymakeplots-0.1.7/pymakeplots/
--rwxr-xr-x   0 tdavis     (501) staff       (20)       87 2020-09-02 10:31:25.000000 pymakeplots-0.1.7/pymakeplots/__init__.py
--rw-r--r--   0 tdavis     (501) staff       (20)    43998 2023-06-15 14:31:16.000000 pymakeplots-0.1.7/pymakeplots/pymakeplots.py
--rwxr-xr-x   0 tdavis     (501) staff       (20)     4448 2020-08-19 16:57:22.000000 pymakeplots-0.1.7/pymakeplots/sauron_colormap.py
-drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-06-22 09:35:05.580833 pymakeplots-0.1.7/pymakeplots.egg-info/
--rw-r--r--   0 tdavis     (501) staff       (20)     1664 2023-06-22 09:35:05.000000 pymakeplots-0.1.7/pymakeplots.egg-info/PKG-INFO
--rw-r--r--   0 tdavis     (501) staff       (20)      315 2023-06-22 09:35:05.000000 pymakeplots-0.1.7/pymakeplots.egg-info/SOURCES.txt
--rw-r--r--   0 tdavis     (501) staff       (20)        1 2023-06-22 09:35:05.000000 pymakeplots-0.1.7/pymakeplots.egg-info/dependency_links.txt
--rw-r--r--   0 tdavis     (501) staff       (20)       68 2023-06-22 09:35:05.000000 pymakeplots-0.1.7/pymakeplots.egg-info/requires.txt
--rw-r--r--   0 tdavis     (501) staff       (20)       12 2023-06-22 09:35:05.000000 pymakeplots-0.1.7/pymakeplots.egg-info/top_level.txt
--rw-r--r--   0 tdavis     (501) staff       (20)        1 2020-09-02 10:52:50.000000 pymakeplots-0.1.7/pymakeplots.egg-info/zip-safe
--rw-r--r--   0 tdavis     (501) staff       (20)       38 2023-06-22 09:35:05.581272 pymakeplots-0.1.7/setup.cfg
--rw-r--r--   0 tdavis     (501) staff       (20)      914 2023-06-22 09:34:20.000000 pymakeplots-0.1.7/setup.py
+drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2024-05-09 16:29:32.374280 pymakeplots-0.2.0/
+-rw-r--r--   0 tdavis     (501) staff       (20)     1077 2020-09-02 10:40:49.000000 pymakeplots-0.2.0/LICENSE.md
+-rw-r--r--   0 tdavis     (501) staff       (20)     1664 2024-05-09 16:29:32.374102 pymakeplots-0.2.0/PKG-INFO
+-rwxr-xr-x   0 tdavis     (501) staff       (20)     1225 2020-09-04 16:00:00.000000 pymakeplots-0.2.0/README.md
+drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2024-05-09 16:29:32.372942 pymakeplots-0.2.0/pymakeplots/
+-rwxr-xr-x   0 tdavis     (501) staff       (20)       87 2020-09-02 10:31:25.000000 pymakeplots-0.2.0/pymakeplots/__init__.py
+-rw-r--r--   0 tdavis     (501) staff       (20)    43686 2024-05-09 16:23:19.000000 pymakeplots-0.2.0/pymakeplots/pymakeplots.py
+-rwxr-xr-x   0 tdavis     (501) staff       (20)     4448 2020-08-19 16:57:22.000000 pymakeplots-0.2.0/pymakeplots/sauron_colormap.py
+drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2024-05-09 16:29:32.373870 pymakeplots-0.2.0/pymakeplots.egg-info/
+-rw-r--r--   0 tdavis     (501) staff       (20)     1664 2024-05-09 16:29:32.000000 pymakeplots-0.2.0/pymakeplots.egg-info/PKG-INFO
+-rw-r--r--   0 tdavis     (501) staff       (20)      315 2024-05-09 16:29:32.000000 pymakeplots-0.2.0/pymakeplots.egg-info/SOURCES.txt
+-rw-r--r--   0 tdavis     (501) staff       (20)        1 2024-05-09 16:29:32.000000 pymakeplots-0.2.0/pymakeplots.egg-info/dependency_links.txt
+-rw-r--r--   0 tdavis     (501) staff       (20)       68 2024-05-09 16:29:32.000000 pymakeplots-0.2.0/pymakeplots.egg-info/requires.txt
+-rw-r--r--   0 tdavis     (501) staff       (20)       12 2024-05-09 16:29:32.000000 pymakeplots-0.2.0/pymakeplots.egg-info/top_level.txt
+-rw-r--r--   0 tdavis     (501) staff       (20)        1 2020-09-02 10:52:50.000000 pymakeplots-0.2.0/pymakeplots.egg-info/zip-safe
+-rw-r--r--   0 tdavis     (501) staff       (20)       38 2024-05-09 16:29:32.374328 pymakeplots-0.2.0/setup.cfg
+-rw-r--r--   0 tdavis     (501) staff       (20)      914 2024-05-09 16:28:45.000000 pymakeplots-0.2.0/setup.py
```

### Comparing `pymakeplots-0.1.7/LICENSE.md` & `pymakeplots-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pymakeplots-0.1.7/PKG-INFO` & `pymakeplots-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymakeplots
-Version: 0.1.7
+Version: 0.2.0
 Home-page: https://github.com/TimothyADavis/pymakeplots
 Author: Timothy A. Davis
 Author-email: DavisT@cardiff.ac.uk
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pymakeplots-0.1.7/README.md` & `pymakeplots-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pymakeplots-0.1.7/pymakeplots/pymakeplots.py` & `pymakeplots-0.2.0/pymakeplots/pymakeplots.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
         self.gal_distance=None
         self.posang=None
         self.vsys=None
         self.transition='CO'
         self.moment1=None
         self.rms=None
         self.flat_cube=None
+        self.obj_ra_pix=None
+        self.obj_dec_pix=None
         self.pbcorr_cube=None
         self.spectralcube=None
         self.mask=None
         self.flat_cube_trim=None
         self.pbcorr_cube_trim=None
         self.mask_trim=None
         self.bmaj=None
@@ -297,29 +299,24 @@
     def rms_estimate(self,cube,chanstart,chanend):
         quarterx=np.array(cube.shape[0]/4.).astype(int)
         quartery=np.array(cube.shape[1]/4.).astype(int)
         return np.nanstd(cube[quarterx*1:3*quarterx,1*quartery:3*quartery,chanstart:chanend])
         
     def get_header_coord_arrays(self,hdr):
 
-        y,x=self.spectralcube.spatial_coordinate_map
+        cd1=self.spectralcube.wcs.pixel_scale_matrix[0,0]*3600
+        cd2=self.spectralcube.wcs.pixel_scale_matrix[1,1]*3600
+        x1=((np.arange(1,hdr['NAXIS1']+1)-(hdr['NAXIS1']//2))*cd1)# + hdr['CRVAL1']
+        y1=((np.arange(1,hdr['NAXIS2']+1)-(hdr['NAXIS1']//2))*cd2)# + hdr['CRVAL2']
 
-        x1=np.median(x[0:hdr['NAXIS2'],0:hdr['NAXIS1']],0).value
-        y1=np.median(y[0:hdr['NAXIS2'],0:hdr['NAXIS1']],1).value
         v1=self.spectralcube.spectral_axis.value
 
         cd3= np.median(np.diff(v1))
-        cd1= np.median(np.diff(x1))
-        
-        if np.any(np.diff(x1) > 359):
-            # we have RA=0 wrap issue
-            x1[x1 > 180]-=360
-            
             
-        return x1,y1,v1,np.abs(cd1*3600),cd3                    
+        return x1,y1,v1,np.abs(cd1),cd3                    
         
     def read_in_a_cube(self,path):
         self.spectralcube=SpectralCube.read(path).with_spectral_unit(u.km/u.s, velocity_convention='radio')#, rest_value=self.restfreq)
 
         hdr=self.spectralcube.header
         cube = np.squeeze(self.spectralcube.filled_data[:,:,:].T).value #squeeze to remove singular stokes axis if present
         cube[np.isfinite(cube) == False] = 0.0
@@ -333,14 +330,16 @@
                 try:
                     beamvals=[self.spectralcube.header['bmaj'],self.spectralcube.header['bmin']]
                     beamtab=Beam(major=np.max(beamvals)*u.deg,minor=np.min(beamvals)*u.deg,pa=self.spectralcube.header['bpa']*u.deg)
                 except:
                     beamtab=False
             
         return cube, hdr, beamtab
+    
+
         
     def read_primary_cube(self,cube):
         
         ### read in cube ###
         datacube,hdr,beam = self.read_in_a_cube(cube)
         
         self.bmaj=beam.major.to(u.arcsec).value
@@ -352,61 +351,52 @@
             self.galname=hdr['OBJECT']
         except:
             self.galname="Galaxy"
             
         
                           
         self.xcoord,self.ycoord,self.vcoord,self.cellsize,self.dv = self.get_header_coord_arrays(hdr)
+        #breakpoint()
         
         
-        
-        try:
-            self.obj_ra=hdr['OBSRA']
-            self.obj_dec=hdr['OBSDEC']
-            if (self.obj_ra > np.max(self.xcoord)) or (self.obj_ra < np.min(self.xcoord)) or (self.obj_dec < np.min(self.ycoord)) or (self.obj_dec > np.max(self.ycoord)):
-                # obsra/dec given in the headers arent in the observed field! Fall back on medians.
-                if not self.silent: print("OBSRA/OBSDEC keywords dont seem correct! Assuming galaxy centre is at pointing centre")
-                self.obj_ra=np.median(self.xcoord)
-                self.obj_dec=np.median(self.ycoord)
-        except:
-            self.obj_ra=np.median(self.xcoord)
-            self.obj_dec=np.median(self.ycoord)
-        
-            
-            
+
         
         if self.dv < 0:
             datacube = np.flip(datacube,axis=2)
             self.dv*=(-1)
             self.vcoord = np.flip(self.vcoord)
             self.flipped=True
         datacube[~np.isfinite(datacube)]=0.0
         
         self.rms= self.rms_estimate(datacube,self.linefree_chans_start,self.linefree_chans_end) 
         return datacube
     
     def prepare_cubes(self):
         
-        self.clip_cube()
+        self.centskycoord=self.spectralcube.wcs.celestial.pixel_to_world(self.xcoord.size//2,self.ycoord.size//2).transform_to('icrs')
+        self.x_skycent=self.centskycoord.ra.value
+        self.y_skycent=self.centskycoord.dec.value
+        if self.obj_ra == None:
+           self.obj_ra=self.x_skycent
+        if self.obj_dec == None:
+           self.obj_dec=self.y_skycent
+        
+        refpos=SkyCoord(self.obj_ra*u.deg,self.obj_dec*u.deg)
+        xpix,ypix=self.spectralcube.wcs.celestial.world_to_pixel(refpos)
             
-        self.mask_trim=self.smooth_mask(self.flat_cube_trim)
+        xoffsetarc=np.interp(xpix,np.arange(self.xcoord.size),self.xcoord)
+        yoffsetarc=np.interp(ypix,np.arange(self.ycoord.size),self.ycoord)
+
         
+        self.clip_cube(xoffsetarc,yoffsetarc)
+            
+        self.mask_trim=self.smooth_mask(self.flat_cube_trim)
         
-        #y,x=self.spectralcube.spatial_coordinate_map
-        #sk=SkyCoord(x,y)
-        # refpos=SkyCoord(self.obj_ra*u.deg,self.obj_dec*u.deg)
-        # sx=SkyCoord(self.xcoord*u.deg,self.obj_dec*u.deg)
-        # self.xc=sx.separation(refpos).to(u.arcsec).value #*  np.cos(np.deg2rad(self.obj_dec)) + self.obj_ra
-        # sy=SkyCoord(self.obj_ra*u.deg,self.ycoord*u.deg)
-        # self.yc=sy.separation(refpos).to(u.arcsec).value #+ self.obj_dec
-        #
-        #
-        # breakpoint()
-        self.xc=(self.xcoord_trim-self.obj_ra)*(-1) * 3600. *  np.cos(np.deg2rad(self.obj_dec))
-        self.yc=(self.ycoord_trim-self.obj_dec) * 3600. 
+
+
         
 
         
 
         if self.gal_distance == None:
             self.gal_distance = self.vsys/70.
             if not self.silent: print("Warning! Estimating galaxy distance using Hubble expansion. Set `gal_distance` if this is not appropriate.")
@@ -447,23 +437,24 @@
 
 
         self.make_moments(axes=np.array([ax1,ax2,ax3]),fits=fits)
         self.make_pvd(axes=ax4,fits=fits)
         self.make_spec(axes=ax5,fits=fits)
         
         ### plotting PA on mom1
-        ypv=self.yc
-        xpv=self.yc*0.0
+        ypv=np.arange(-np.max(self.yc),np.max(self.yc),20)
+        xpv=ypv*0.0
         ang=self.posang
         c = np.cos(np.deg2rad(ang))
         s = np.sin(np.deg2rad(ang))
         x2 =  c*xpv - s*ypv
         y2 =  s*xpv + c*ypv
+        ax2.scatter(0,0,facecolors='none',edgecolors='k')
         ax2.plot(x2,y2,'k--')
-
+        #breakpoint()
 
         ###### make summary box
         
         rjustnum=35
 
         c = ICRS(self.obj_ra*u.degree, self.obj_dec*u.degree)
 
@@ -474,15 +465,15 @@
         thetext += ("Dist: "+str(round(self.gal_distance,1))+" Mpc")+'\n'
         if self.gal_distance == self.vsys/70.:
             thetext+=("(Est. from Vsys)")
 
 
 
         at2 = AnchoredText(thetext,
-                           loc='upper right', prop=dict(size=30,multialignment='right'), frameon=False,
+                           loc='upper right', prop=dict(size=25,multialignment='right'), frameon=False,
                            bbox_transform=textaxes.transAxes
                            )
         textaxes.add_artist(at2)
 
 
 
         if pdf:
@@ -527,15 +518,15 @@
 
         
         if self.gal_distance != None and not self.all_axes_physical:
             self.scalebar(axes[i]) # plot onto last axes
 
                     
         if pdf:
-            plt.savefig(self.galname+"_moment"+"".join(mom.astype(np.str))+".pdf", bbox_inches = 'tight')
+            plt.savefig(self.galname+"_moment"+"".join(mom.astype(str))+".pdf", bbox_inches = 'tight')
             plt.close()
         else:
             if not outsideaxis:
                 plt.show()
                 plt.close()
     
     def scalebar(self,ax,loc='lower right'):
@@ -549,26 +540,30 @@
         if barlength_arc > 0.3*np.abs(self.xc[-1]-self.xc[0]): # go to 1 pc rounding
             barlength_pc = np.ceil((np.abs(self.xc[-1]-self.xc[0])*4.84*self.gal_distance)/10.)*1
             barlength_arc=  barlength_pc/(4.84*self.gal_distance)
             
             
         
         if np.log10(barlength_pc) > 3:
-            label=(barlength_pc/1e3).astype(np.str)+ " kpc"
+            label=(barlength_pc/1e3).astype(str)+ " kpc"
         else:
-            label=barlength_pc.astype(int).astype(np.str)+ " pc"
+            label=barlength_pc.astype(int).astype(str)+ " pc"
             
         asb = AnchoredSizeBar(ax.transData,  barlength_arc,   label,  loc=loc,  pad=0.25, borderpad=0.5, sep=5, frameon=False)
         ax.add_artist(asb)
         
         
         
         
             
-    def clip_cube(self):
+    def clip_cube(self,xoffsetarc,yoffsetarc):
+        
+        #
+        
+        
         
         if self.chans2do == None:
             # use the mask to try and guess the channels with signal.
             mask_cumsum=np.nancumsum((self.pbcorr_cube > self.rmsfac*self.rms).sum(axis=0).sum(axis=0))
             w_low,=np.where(mask_cumsum/np.max(mask_cumsum) < 0.02)
             w_high,=np.where(mask_cumsum/np.max(mask_cumsum) > 0.98)
             
@@ -581,26 +576,27 @@
             self.vsys=((self.pbcorr_cube*(self.pbcorr_cube > self.rmsfac*self.rms)).sum(axis=0).sum(axis=0)*self.vcoord).sum()/((self.pbcorr_cube*(self.pbcorr_cube > self.rmsfac*self.rms)).sum(axis=0).sum(axis=0)).sum()
         
         if self.imagesize != None:
             if np.array(self.imagesize).size == 1:
                 self.imagesize=[self.imagesize,self.imagesize]
             
 
-            wx,=np.where((np.abs((self.xcoord-self.obj_ra)*3600.) <= self.imagesize[0]/np.cos(np.deg2rad(self.obj_dec))))
-            wy,=np.where((np.abs((self.ycoord-self.obj_dec)*3600.) <= self.imagesize[1]))
-            self.spatial_trim=[np.min(wx),np.max(wx),np.min(wy),np.max(wy)]        
+            wx,=np.where(np.abs(self.xcoord-xoffsetarc) <= self.imagesize[0])
+            wy,=np.where(np.abs(self.ycoord-yoffsetarc) <= self.imagesize[1])
+            self.spatial_trim=[np.min(wx),np.max(wx),np.min(wy),np.max(wy)]  
+                  
         
         if self.spatial_trim == None:
             
             mom0=(self.pbcorr_cube > self.rmsfac*self.rms).sum(axis=2)
             mom0[mom0>0]=1
             
-            cumulative_x = np.nancumsum(mom0.sum(axis=1),dtype=np.float)
+            cumulative_x = np.nancumsum(mom0.sum(axis=1),dtype=float)
             cumulative_x /= np.nanmax(cumulative_x)
-            cumulative_y = np.nancumsum(mom0.sum(axis=0),dtype=np.float)
+            cumulative_y = np.nancumsum(mom0.sum(axis=0),dtype=float)
             cumulative_y /= np.nanmax(cumulative_y)
             
             wx_low,=np.where(cumulative_x < 0.02)
             if wx_low.size ==0: wx_low=np.array([0])
             wx_high,=np.where(cumulative_x > 0.98)
             if wx_high.size ==0: wx_high=np.array([cumulative_x.size])
             wy_low,=np.where(cumulative_y < 0.02)
@@ -612,24 +608,24 @@
             
             beam_in_pix = int(np.ceil(self.bmaj/self.cellsize))
             
 
             self.spatial_trim = [np.clip(np.max(wx_low) - 2*beam_in_pix,0,self.xcoord.size),np.clip(np.min(wx_high) + 2*beam_in_pix,0,self.xcoord.size)\
                                 , np.clip(np.max(wy_low) - 2*beam_in_pix,0,self.ycoord.size), np.clip(np.min(wy_high) + 2*beam_in_pix,0,self.ycoord.size)]
             
-        #breakpoint()
         #print(np.where(np.isclose(self.xcoord-self.obj_ra,0,atol=self.cellsize/3600)))   
         self.flat_cube_trim=self.flat_cube[self.spatial_trim[0]:self.spatial_trim[1],self.spatial_trim[2]:self.spatial_trim[3],self.chans2do[0]:self.chans2do[1]]
         self.pbcorr_cube_trim=self.pbcorr_cube[self.spatial_trim[0]:self.spatial_trim[1],self.spatial_trim[2]:self.spatial_trim[3],self.chans2do[0]:self.chans2do[1]]
         #self.mask_trim=self.mask[self.spatial_trim[0]:self.spatial_trim[1],self.spatial_trim[2]:self.spatial_trim[3],self.chans2do[0]:self.chans2do[1]] 
         self.spectralcube=self.spectralcube[self.chans2do[0]:self.chans2do[1],self.spatial_trim[2]:self.spatial_trim[3],self.spatial_trim[0]:self.spatial_trim[1]] 
         self.xcoord_trim=self.xcoord[self.spatial_trim[0]:self.spatial_trim[1]]
         self.ycoord_trim=self.ycoord[self.spatial_trim[2]:self.spatial_trim[3]]
         self.vcoord_trim=self.vcoord[self.chans2do[0]:self.chans2do[1]]  
-            
+        self.xc=(self.xcoord_trim-xoffsetarc)*(-1) 
+        self.yc=(self.ycoord_trim-yoffsetarc)    
            
             
     
 
     def colorbar(self,mappable,ticks=None):
         ax = mappable.axes
         fig = ax.figure
@@ -639,19 +635,19 @@
         cax.xaxis.set_ticks_position("top")
         cax.xaxis.set_label_position('top')
         return cb         
             
         
     def add_beam(self,ax):    
         if self.all_axes_physical:
-            ae = AnchoredEllipse(ax.transData, width=self.ang2kpctrans(self.bmaj), height=self.ang2kpctrans(self.bmin), angle=self.bpa,
+            ae = AnchoredEllipse(ax.transData, width=self.ang2kpctrans(self.bmaj), height=self.ang2kpctrans(self.bmin), angle=self.bpa+90,
                              loc='lower left', pad=0.5, borderpad=0.4,
                              frameon=False)
         else:
-            ae = AnchoredEllipse(ax.transData, width=self.bmaj, height=self.bmin, angle=self.bpa,
+            ae = AnchoredEllipse(ax.transData, width=self.bmaj, height=self.bmin, angle=self.bpa+90,
                              loc='lower left', pad=0.5, borderpad=0.4,
                              frameon=False)                   
         ae.ellipse.set_edgecolor('black')
         ae.ellipse.set_facecolor('none')
         ae.ellipse.set_linewidth(1.5)
         ax.add_artist(ae)
         
@@ -671,18 +667,18 @@
             if minmom0==maxmom0:
                 minmom0=1e-5
             levs=np.linspace(minmom0,maxmom0,10)
         else:
             levs=np.linspace(0,1,10)
             mom0-=1    
             
-            
-         
+        #mom0[mom0<minmom0]=np.nan    
+        #breakpoint() 
         im1=ax1.contourf(self.xc,self.yc,mom0.T,levels=levs,cmap=newcmp)
-
+        #im1=ax1.pcolormesh(self.xc,self.yc,mom0.T,cmap=newcmp,vmin=minmom0,vmax=maxmom0)
             
         if self.all_axes_physical:
             ax1.set_xlabel('RA offset (kpc)')
             if first: ax1.set_ylabel('Dec offset (kpc)')
         else:
             ax1.set_xlabel('RA offset (")')
             if first: ax1.set_ylabel('Dec offset (")')
@@ -821,17 +817,17 @@
                     
         if self.fits:
             self.write_fits(mom2.T,2)
       
       
     def write_fits(self,array,whichmoment):
         if self.fits == True:
-            filename=self.galname+"_mom"+"".join(np.array([whichmoment]).astype(np.str))+".fits"
+            filename=self.galname+"_mom"+"".join(np.array([whichmoment]).astype(str))+".fits"
         else:
-            filename=self.fits+"_mom"+"".join(np.array([whichmoment]).astype(np.str))+".fits"
+            filename=self.fits+"_mom"+"".join(np.array([whichmoment]).astype(str))+".fits"
         
   
         newhdu = fits.PrimaryHDU(array)
 
         newhdu.header['CRPIX1']=self.spectralcube.header['CRPIX1']
         newhdu.header['CRVAL1']=self.spectralcube.header['CRVAL1']
         newhdu.header['CDELT1']=self.spectralcube.header['CDELT1']
@@ -964,18 +960,18 @@
                      # posang should be lt 180
                     if self.posang > 180: self.posang -= 180
             if not self.silent: print("PA estimate (degrees): ",np.round(self.posang,1))        
         
                     
         centpix_x=np.where(np.isclose(self.xc,0.0,atol=self.cellsize/1.9))[0]
         centpix_y=np.where(np.isclose(self.yc,0.0,atol=self.cellsize/1.9))[0]
-        
+        #breakpoint()
 
 
-        rotcube= rotateImage(self.pbcorr_cube_trim*self.mask_trim,90-self.posang,[centpix_x[0],centpix_y[0]])
+        rotcube= rotateImage(self.pbcorr_cube_trim*self.mask_trim,90-self.posang,[centpix_y[0],centpix_x[0]])
 
 
         pvd=rotcube[:,np.array(rotcube.shape[1]//2-self.pvdthick).astype(int):np.array(rotcube.shape[1]//2+self.pvdthick).astype(int),:].sum(axis=1)
         
 
         
         if self.posang < 180:
@@ -1042,15 +1038,15 @@
             self.set_rc_params(mult=0.75)   
             fig,axes=plt.subplots(1,figsize=(7,5))
             outsideaxis=0
         else:
             outsideaxis=1
         spec=self.pbcorr_cube[self.spatial_trim[0]:self.spatial_trim[1],self.spatial_trim[2]:self.spatial_trim[3],:].sum(axis=0).sum(axis=0)
         spec_mask=(self.pbcorr_cube_trim*self.mask_trim).sum(axis=0).sum(axis=0)
-    
+        ylab="Unknown"
         #breakpoint()
         if (''.join(self.bunit.split())).lower() == "Jy/beam".lower():
             
             spec*=1/self.beam_area()
             spec_mask*=1/self.beam_area()
             
             if spec_mask.max() < 1:
@@ -1117,8 +1113,8 @@
        t.write(filename+"_spec.csv", format='csv',overwrite=True)
        
        t1 = Table([vmask,specmask],names=('Velocity (km/s)', descrip))   
        t1.write(filename+"_specmask.csv", format='csv',overwrite=True)
        
        
     
-           
+
```

### Comparing `pymakeplots-0.1.7/pymakeplots/sauron_colormap.py` & `pymakeplots-0.2.0/pymakeplots/sauron_colormap.py`

 * *Files identical despite different names*

### Comparing `pymakeplots-0.1.7/pymakeplots.egg-info/PKG-INFO` & `pymakeplots-0.2.0/pymakeplots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymakeplots
-Version: 0.1.7
+Version: 0.2.0
 Home-page: https://github.com/TimothyADavis/pymakeplots
 Author: Timothy A. Davis
 Author-email: DavisT@cardiff.ac.uk
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pymakeplots-0.1.7/setup.py` & `pymakeplots-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
  
 setup(name='pymakeplots',
-       version='0.1.7',
+       version='0.2.0',
        description='',
        url='https://github.com/TimothyADavis/pymakeplots',
        author='Timothy A. Davis',
        author_email='DavisT@cardiff.ac.uk',
        long_description=long_description,
        long_description_content_type="text/markdown",
        license='MIT',
```

