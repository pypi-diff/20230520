# Comparing `tmp/nico_sc_sp-0.0.2.tar.gz` & `tmp/nico-sc-sp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nico_sc_sp-0.0.2.tar", last modified: Mon May 15 20:35:39 2023, max compression
+gzip compressed data, was "nico-sc-sp-0.0.3.tar", last modified: Sat May 20 19:36:26 2023, max compression
```

## Comparing `nico_sc_sp-0.0.2.tar` & `nico-sc-sp-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 agrawal    (503) staff       (20)        0 2023-05-15 20:35:39.223164 nico_sc_sp-0.0.2/
--rw-r--r--   0 agrawal    (503) staff       (20)      947 2023-05-15 20:35:39.222908 nico_sc_sp-0.0.2/PKG-INFO
--rw-rw-r--   0 agrawal    (503) staff       (20)      340 2023-05-15 20:21:18.000000 nico_sc_sp-0.0.2/README.md
-drwxr-xr-x   0 agrawal    (503) staff       (20)        0 2023-05-15 20:35:39.219192 nico_sc_sp-0.0.2/nico/
--rwxrwxrwx   0 agrawal    (503) staff       (20)    36141 2023-02-23 13:01:40.000000 nico_sc_sp-0.0.2/nico/Spatial_Annotations.py
--rw-r--r--   0 agrawal    (503) staff       (20)    87490 2023-05-15 17:00:52.000000 nico_sc_sp-0.0.2/nico/Spatial_Covariations.py
--rw-r--r--   0 agrawal    (503) staff       (20)    40181 2023-04-17 16:02:34.000000 nico_sc_sp-0.0.2/nico/Spatial_Interactions.py
--rw-r--r--   0 agrawal    (503) staff       (20)    87298 2023-05-04 09:21:53.000000 nico_sc_sp-0.0.2/nico/Spatial_Pathways_integrated_NMFGene_Weight_celltypePairwise_case3a_RidgeCV_V4.py
--rw-rw-r--   0 agrawal    (503) staff       (20)     3695 2023-05-15 16:55:34.000000 nico_sc_sp-0.0.2/nico/__init__.py
-drwxr-xr-x   0 agrawal    (503) staff       (20)        0 2023-05-15 20:35:39.220750 nico_sc_sp-0.0.2/nico/utilities/
--rwxrwxrwx   0 agrawal    (503) staff       (20)     9494 2022-03-29 11:28:38.000000 nico_sc_sp-0.0.2/nico/utilities/SCTransform.py
--rw-rw-r--   0 agrawal    (503) staff       (20)      742 2023-05-15 15:35:51.000000 nico_sc_sp-0.0.2/nico/utilities/__init__.py
--rw-rw-r--   0 agrawal    (503) staff       (20)    17782 2023-05-15 15:35:03.000000 nico_sc_sp-0.0.2/nico/utilities/pyliger_utilities.py
-drwxr-xr-x   0 agrawal    (503) staff       (20)        0 2023-05-15 20:35:39.222531 nico_sc_sp-0.0.2/nico_sc_sp.egg-info/
--rw-r--r--   0 agrawal    (503) staff       (20)      947 2023-05-15 20:35:39.000000 nico_sc_sp-0.0.2/nico_sc_sp.egg-info/PKG-INFO
--rw-r--r--   0 agrawal    (503) staff       (20)      469 2023-05-15 20:35:39.000000 nico_sc_sp-0.0.2/nico_sc_sp.egg-info/SOURCES.txt
--rw-r--r--   0 agrawal    (503) staff       (20)        1 2023-05-15 20:35:39.000000 nico_sc_sp-0.0.2/nico_sc_sp.egg-info/dependency_links.txt
--rw-r--r--   0 agrawal    (503) staff       (20)       14 2023-05-15 20:35:39.000000 nico_sc_sp-0.0.2/nico_sc_sp.egg-info/requires.txt
--rw-r--r--   0 agrawal    (503) staff       (20)        5 2023-05-15 20:35:39.000000 nico_sc_sp-0.0.2/nico_sc_sp.egg-info/top_level.txt
--rw-r--r--   0 agrawal    (503) staff       (20)       38 2023-05-15 20:35:39.223273 nico_sc_sp-0.0.2/setup.cfg
--rw-rw-r--   0 agrawal    (503) staff       (20)     1259 2023-05-15 20:33:14.000000 nico_sc_sp-0.0.2/setup.py
+drwxr-xr-x   0 agrawal    (503) staff       (20)        0 2023-05-20 19:36:26.091205 nico-sc-sp-0.0.3/
+-rw-r--r--   0 agrawal    (503) staff       (20)     1683 2023-05-20 19:36:26.090952 nico-sc-sp-0.0.3/PKG-INFO
+-rw-rw-r--   0 agrawal    (503) staff       (20)     1076 2023-05-17 10:45:23.000000 nico-sc-sp-0.0.3/README.md
+drwxr-xr-x   0 agrawal    (503) staff       (20)        0 2023-05-20 19:36:26.088195 nico-sc-sp-0.0.3/nico/
+-rwxrwxrwx   0 agrawal    (503) staff       (20)    37217 2023-05-20 19:19:42.000000 nico-sc-sp-0.0.3/nico/Spatial_Annotations.py
+-rw-r--r--   0 agrawal    (503) staff       (20)    80363 2023-05-20 19:01:37.000000 nico-sc-sp-0.0.3/nico/Spatial_Covariations.py
+-rw-r--r--   0 agrawal    (503) staff       (20)    43632 2023-05-20 19:23:39.000000 nico-sc-sp-0.0.3/nico/Spatial_Interactions.py
+-rw-rw-r--   0 agrawal    (503) staff       (20)     3707 2023-05-20 15:13:45.000000 nico-sc-sp-0.0.3/nico/__init__.py
+drwxr-xr-x   0 agrawal    (503) staff       (20)        0 2023-05-20 19:36:26.089148 nico-sc-sp-0.0.3/nico/utilities/
+-rwxrwxrwx   0 agrawal    (503) staff       (20)     9494 2022-03-29 11:28:38.000000 nico-sc-sp-0.0.3/nico/utilities/SCTransform.py
+-rw-rw-r--   0 agrawal    (503) staff       (20)      742 2023-05-15 15:35:51.000000 nico-sc-sp-0.0.3/nico/utilities/__init__.py
+-rw-rw-r--   0 agrawal    (503) staff       (20)    17782 2023-05-15 15:35:03.000000 nico-sc-sp-0.0.3/nico/utilities/pyliger_utilities.py
+drwxr-xr-x   0 agrawal    (503) staff       (20)        0 2023-05-20 19:36:26.090626 nico-sc-sp-0.0.3/nico_sc_sp.egg-info/
+-rw-r--r--   0 agrawal    (503) staff       (20)     1683 2023-05-20 19:36:26.000000 nico-sc-sp-0.0.3/nico_sc_sp.egg-info/PKG-INFO
+-rw-r--r--   0 agrawal    (503) staff       (20)      383 2023-05-20 19:36:26.000000 nico-sc-sp-0.0.3/nico_sc_sp.egg-info/SOURCES.txt
+-rw-r--r--   0 agrawal    (503) staff       (20)        1 2023-05-20 19:36:26.000000 nico-sc-sp-0.0.3/nico_sc_sp.egg-info/dependency_links.txt
+-rw-r--r--   0 agrawal    (503) staff       (20)       91 2023-05-20 19:36:26.000000 nico-sc-sp-0.0.3/nico_sc_sp.egg-info/requires.txt
+-rw-r--r--   0 agrawal    (503) staff       (20)        5 2023-05-20 19:36:26.000000 nico-sc-sp-0.0.3/nico_sc_sp.egg-info/top_level.txt
+-rw-r--r--   0 agrawal    (503) staff       (20)       38 2023-05-20 19:36:26.091281 nico-sc-sp-0.0.3/setup.cfg
+-rw-rw-r--   0 agrawal    (503) staff       (20)     1361 2023-05-20 19:36:07.000000 nico-sc-sp-0.0.3/setup.py
```

### Comparing `nico_sc_sp-0.0.2/nico/Spatial_Annotations.py` & `nico-sc-sp-0.0.3/nico/Spatial_Annotations.py`

 * *Files 10% similar despite different names*

```diff
@@ -80,20 +80,18 @@
      t1=d1[index_2]
      s1=k_index_1[index_2]
      for index_1 in s1:
         t2=d2[index_1]
         s2=k_index_2[index_1]
         if index_2 in s2:
             p1,p2=find_match_index_in_dist(t1,t2,s1,s2,index_1,index_2)
-            #print('a',temp1[index_1],temp2[index_2])
             mutual_1.append(index_1)
             mutual_2.append(index_2)
             dist_1.append(p1)
             dist_2.append(p2)
-    #print(mutual_1,dist_1)
 
     a1=np.array(mutual_1)
     a2=np.array(mutual_2)
     dist_1=np.array(dist_1)
     dist_2=np.array(dist_2)
     a1=sp_barcode[a1]
     a2=sc_barcode[a2]
@@ -261,17 +259,16 @@
         #print(i,spatialcell_cluid)
         mat3[0,col]+=1
 
 
     anchorFreqRow=mat3/total_in_row
     anchorFreqCol=mat1/total_in_col
 
-    print("SC",total_in_col,np.sum(total_in_col))
-    print("SP",total_in_row,np.sum(total_in_row))
-    print(data.shape)
+    #print("SC",total_in_col,np.sum(total_in_col))
+    #print("SP",total_in_row,np.sum(total_in_row))
 
     save_anchors={}
     for i in range(len(data)):
             spatialcell_cluid=d_spatial[data[i,0]]
             singlecell_cluid=d_single[data[i,1]]
             #print(i,spatialcell_cluid,singlecell_cluid)
             col=d_spatial_cluster[spatialcell_cluid]
@@ -331,15 +328,15 @@
         if len(temp)==1:
             low_anc_ct=temp[0]
             if low_anc_ct not in low_anchors_spatial_clusters:
                 low_anchors_spatial_clusters[low_anc_ct]=[key]
             else:
                 low_anchors_spatial_clusters[low_anc_ct].append(key)
 
-    print(low_anchors_spatial_clusters)
+    #print("low anchors",low_anchors_spatial_clusters)
     #{'KCs': ['c11', 'c7'], 'Stellatecells': ['c12'], 'Cholangiocytes': ['c16'], 'Bcells': ['c17'], 'LSECs': ['c18', 'c6']}
 
 
     fw.close()
     fw=open(input.savepath+"spatial_annotation_along_SC.dat",'w')
     good_anchors={}
     tt=[]
@@ -375,114 +372,140 @@
                         else:
                             good_anchors[name]+=1
 
         fw.write(str(i)+'\t'+newcname2[i]+'\tF='+str('%0.3f'%af)+',\t'+found+'\n')
     fw.close()
 
 
-    print(len(np.unique(tt)))
-    print(len(np.unique(list(save_anchors.keys()))))
+    #print(len(np.unique(tt)))
+    #print(len(np.unique(list(save_anchors.keys()))))
 
     c=0
     for key in good_anchors:
         c+=good_anchors[key]
 
     count=0
     ca={}
     for key in save_anchors:
         list_of_anchors=save_anchors[key]
         count+=len(list_of_anchors)
         for j in range(len(list_of_anchors)):
             ca[list_of_anchors[j]]=1
 
-    print('good anchors',len(good_anchors),c,'\t\tsave',len(ca),count)
-
 
 
 
 
     colname=['total # of sc', 'total # of sp']
     cname1=['anchorFreq']+list(input.lsc[0])
 
 
-
-
-
-    #print(cname2)
-    #fig,ax=plt.subplots(1,2,figsize=(20,10))
-    fig=plt.figure(figsize=(15,10))
-    gs = gridspec.GridSpec(1, 2, width_ratios=[1, 10])
-    ax0=plt.subplot(gs[0])
-    ax1=plt.subplot(gs[1])
-    fig.suptitle('MNN K = ' + str(input.KNN),fontsize=12)
+    fig=plt.subplots(1,1,figsize=(12,10))
+    #fig=plt.figure(figsize=(15,10))
+    #gs = gridspec.GridSpec(1, 2, width_ratios=[1, 10])
+    #ax0=plt.subplot(gs[0])
+    #ax1=plt.subplot(gs[1])
     #snn.heatmap(ax=ax0,data=mat1,annot=True, fmt='d',xticklabels=colname, annot_kws={"size": 5},yticklabels=cname1)
 
-    snn.heatmap(ax=ax1,data=mat2,annot=True, fmt='0.2f',xticklabels=cname2, annot_kws={"size": 5},yticklabels=cname1)
+    snn.heatmap(data=mat2,annot=True, fmt='0.2f',xticklabels=cname2, annot_kws={"size": 5},yticklabels=cname1)
     plt.xlabel('Spatial cell clusters')
     plt.ylabel('Single cell clusters')
+    plt.title('MNN K = ' + str(input.KNN),fontsize=12)
 
     #plt.title('R = '+str(radius)+', C='+str(lambda_c))
     #g.xaxis.set_ticks_position("top")
     plt.tight_layout()
-    fig.savefig(input.savepath+'Res_MNN_K_'+str(input.KNN)+'.png',dpi=300)
+    plt.savefig(input.savepath+'Res_MNN_K_'+str(input.KNN)+'.png',dpi=300)
 
     return good_anchors
 
 
 
 
-def built_MNN_matrix_between_sc_and_sp(input):
-#def main():
+def find_anchor_cells_between_ref_and_query(ref_cluster_file,ref_CTname_file,refpath='./inputSC/',quepath='./inputSP/',ref_h5ad='./inputSC/scTransform_singleCell.h5ad',
+que_h5ad='./inputSP/spatial_data_with_many_guided_cluster_resolutions.h5ad',delimiter=',',neigh=50,no_of_pc=50,number_of_iteration_in_degree_based_annotations=3,
+minkowski_order=2,MNN_across_spatial_clusters_dispersion_cutoff=0.15,guided_spatial_cluster_leiden_tag='leiden05'):
+
+
     '''
-    scdatapath='./inputSC/'
-    spdatapath='./inputSP/'
-    outputFolder=spdatapath+'find_MNN/'
-    neigh=50
-    no_of_pc=50
+    Default parameters are following:
+
+    There should be no header information in cell type filename (ref_CTname_file)
+    The cluster filenaname (ref_cluster_file) should have the header information
+    The output annotation file will be saved in quepath/MNN_based_annotations/*
+    First time run to find the good anchored cells
+    Second time run to find the annotations based on the highest degree of spatial cell neighbors
+
+    ref_cluster_file #give a scRNAseq cluster file
+    ref_CTname_file #give a scRNAseq cluster cell type name (first column is cluster id, and second column is cell type name)
+    refpath='./inputSC/'   #all the output related to scRNAseq will save it here
+    quepath='./inputSP/'   #all the output related to spatial data will save it here
+    ref_h5ad='./inputSC/scTransform_singleCell.h5ad'  #input scTransform of common gene scRNAseq data in h5ad format
+    que_h5ad='./inputSP/spatial_data_with_many_guided_cluster_resolutions.h5ad' #input scTransform of common gene spatial data in h5ad format
+    delimiter=','  #This delimiter used in the ref_CTname_file
+    neigh=50  # Use to find the KNN
+    no_of_pc=50 #No. of principal components used to find the mutual nearest neighbor step
+    number_of_iteration_in_degree_based_annotations=3 #degree based annotations performed 3 times
+    minkowski_order=2  #2 means euclidean distance,1 means manhattan distance
+    MNN_across_spatial_clusters_dispersion_cutoff=0.15 #remove the noisy anchors if they belong to <0.15 % population of any given spatial cluster
+    guided_spatial_cluster_leiden_tag='leiden05'   #default value of spatial leiden cluster at resolution 0.5
+
     '''
 
-    spatial_deg_annotation_output_clustername=input.spatial_annotation_output_fname+'_cluster.csv'
-    spatial_deg_annotation_output_celltypename=input.spatial_annotation_output_fname+'_ct_name.dat'
-    outputFolder=input.outputFolder
-    neigh=input.neigh
-    no_of_pc=input.no_of_pc
-    MNN_across_spatial_clusters_dispersion_cutoff=input.MNN_across_spatial_clusters_dispersion_cutoff
-    resolutionWiseClustering=input.resolutionWiseClustering
-    minkowski_order=input.minkowski_order
-    number_of_iteration_in_degree_based_annotations=input.number_of_iteration_in_degree_based_annotations
+
+
+
+
+    df=pd.read_csv(ref_cluster_file)
+    sc_cluster=df.to_numpy()
+    df=pd.read_csv(ref_CTname_file,sep=delimiter,header=None)
+    sc_ct_name=df.to_numpy()
+
+    spatial_annotation_output_fname='deg_annotation_spatial'
+    spatial_deg_annotation_output_clustername=spatial_annotation_output_fname+'_cluster.csv'
+    spatial_deg_annotation_output_celltypename=spatial_annotation_output_fname+'_ct_name.dat'
+
+    outputFolder=quepath+'MNN_based_annotations/'
+
 
     create_directory(outputFolder)
 
     #method='gauss'
     method='umap'
 
-    annotation_spatial_barcode_id= input.sp_cluster[:,0]
-    annotation_spatial_cluster_id= input.sp_cluster[:,1]
-    #print(np.unique(annotation_spatial_cluster_id))
-    spatialcell_unique_clustername=input.sp_ct_name[:,1]
-    spatialcell_unique_clusterid=input.sp_ct_name[:,0]
+    adata=sc.read_h5ad(que_h5ad)
+    df=adata.obs[guided_spatial_cluster_leiden_tag]#.to_csv(spatialclusterFilename,header=True)
+    #data=df.to_numpy()
+    #df.to_csv('ankit.csv',header=True)
+
+
+    annotation_spatial_barcode_id= df.index.to_numpy()
+    annotation_spatial_cluster_id= df.to_numpy()
+    spatialcell_unique_clustername=[]
+    spatialcell_unique_clusterid=sorted(list(np.unique(annotation_spatial_cluster_id)))
     d={}
-    for i in range(len(input.sp_ct_name)):
-        #print(i,input.sp_ct_name[i,0],type(input.sp_ct_name[i,0]),input.sp_ct_name[i,1])
-        d[input.sp_ct_name[i,0]]=input.sp_ct_name[i,1]
+    for i in range(len(spatialcell_unique_clusterid)):
+        name='c'+str(spatialcell_unique_clusterid[i])
+        d[spatialcell_unique_clusterid[i]]=name
+        spatialcell_unique_clustername.append(name)
     annotation_spatial_celltypename=[]
     for i in range(len(annotation_spatial_cluster_id)):
         #print(i,annotation_spatial_cluster_id[i],type(annotation_spatial_cluster_id[i]))
         annotation_spatial_celltypename.append(d[annotation_spatial_cluster_id[i]])
     annotation_spatial_celltypename=np.array(annotation_spatial_celltypename)
+    spatialcell_unique_clustername=np.array(spatialcell_unique_clustername)
 
 
-
-    annotation_singlecell_barcode_id=input.sc_cluster[:,0]
-    annotation_singlecell_cluster_id=input.sc_cluster[:,1]
-    singlecell_unique_clustername=input.sc_ct_name[:,1]
-    singlecell_unique_clusterid=input.sc_ct_name[:,0]
+    annotation_singlecell_barcode_id=sc_cluster[:,0]
+    annotation_singlecell_cluster_id=sc_cluster[:,1]
+    singlecell_unique_clustername=sc_ct_name[:,1]
+    singlecell_unique_clusterid=sc_ct_name[:,0]
     d={}
-    for i in range(len(input.sc_ct_name)):
-        d[input.sc_ct_name[i,0]]=input.sc_ct_name[i,1]
+    for i in range(len(sc_ct_name)):
+        d[sc_ct_name[i,0]]=sc_ct_name[i,1]
     annotation_singlecell_celltypename=[]
     for i in range(len(annotation_singlecell_cluster_id)):
         annotation_singlecell_celltypename.append(d[annotation_singlecell_cluster_id[i]])
     annotation_singlecell_celltypename=np.array(annotation_singlecell_celltypename)
 
 
     '''
@@ -528,63 +551,61 @@
         index_sp,index_sc=find_index(sp_genename,sc_genename)
 
         print('before sct normalization of single cell',len(index_sp),len(index_sc))
         ad_sc=ad_sc_ori[:,index_sc].copy()
         ad_sp=ad_sp_ori[:,index_sp].copy()
         '''
 
-        if os.path.isfile(input.spfname):
-            filesize = os.path.getsize(input.spfname)
+        if os.path.isfile(que_h5ad):
+            filesize = os.path.getsize(que_h5ad)
             if filesize>0:
-                sct_ad_sp=sc.read_h5ad(input.spfname)
+                sct_ad_sp=sc.read_h5ad(que_h5ad)
         else:
             print("your input is wrong")
             sct_ad_sp = SCTransform(ad_sp,min_cells=5,gmean_eps=1,n_genes=500,n_cells=None, #use all cells
                         bin_size=500,bw_adjust=3,inplace=False)
             sct_ad_sp.write_h5ad(fname)
 
         #fname=scdatapath+'scTransform_singleCell_si.h5ad'
-        if os.path.isfile(input.scfname):
-            filesize = os.path.getsize(input.scfname)
+        if os.path.isfile(ref_h5ad):
+            filesize = os.path.getsize(ref_h5ad)
             if filesize>0:
-                sct_ad_sc=sc.read_h5ad(input.scfname)
+                sct_ad_sc=sc.read_h5ad(ref_h5ad)
         else:
             print("your input is wrong")
             sct_ad_sc = SCTransform(ad_sc,min_cells=5,gmean_eps=1,n_genes=500,n_cells=None, #use all cells
                         bin_size=500,bw_adjust=3,inplace=False)
             sct_ad_sc.write_h5ad(fname)
 
 
 
         sp_genename=sct_ad_sp.var_names.to_numpy()
         sc_genename=sct_ad_sc.var_names.to_numpy()
         index_sp,index_sc=find_index(sp_genename,sc_genename)
-        print('after sct normalization of single cell',len(index_sp),len(index_sc))
 
         ad_sp_ori=sct_ad_sp[:,index_sp].copy()
         ad_sc_ori=sct_ad_sc[:,index_sc].copy()
 
         ad_sc_ori.write_h5ad(outputFolder+'final_sct_sc.h5ad')
         ad_sp_ori.write_h5ad(outputFolder+'final_sct_sp.h5ad')
 
-        print('\n\n 3 sct Shared Common Gene PC space')
         #ad_sp_ori=ad_sp_ori[0:100,:]
         #ad_sc_ori=ad_sc_ori[0:100,:]
         #print(ad_sc_ori)
         #print(ad_sp_ori)
         input_sp,input_sc,sp_barcode,sc_barcode=sct_return_sc_sp_in_shared_common_PC_space(ad_sp_ori,ad_sc_ori,no_of_pc,method)
-        print('sp',input_sp.shape,'\nsc',input_sc.shape)
+        #print('sp',input_sp.shape,'\nsc',input_sc.shape)
 
 
         if os.path.isfile(fname):
             pass
         else:
             n_jobs=-1
             #input_sp=input_sp[0:20]
-            print(input_sp.shape)
+            #print(input_sp.shape)
             k_dist,k_index = cKDTree(input_sp).query(x=input_sp, k=neigh, p=minkowski_order,workers=n_jobs)
             fw=open(fname,'w')
             for i in range(len(k_index)):
                 for j in range(len(k_index[i])):
                     id=k_index[i,j]
                     fw.write(sp_barcode[id]+',')
                 fw.write('\n')
@@ -618,63 +639,51 @@
         input['savepath']=outputFolder
         input['KNN']=neigh
         input['KNNfilename']=fname
         input['ad_sp']=ad_sp_ori
         input['spatial_deg_annotation_output_clustername']=spatial_deg_annotation_output_clustername
         input['spatial_deg_annotation_output_celltypename']=spatial_deg_annotation_output_celltypename
         input['MNN_across_spatial_clusters_dispersion_cutoff']=MNN_across_spatial_clusters_dispersion_cutoff
-        input['resolutionWiseClustering']=resolutionWiseClustering
         input['number_of_iteration_in_degree_based_annotations']=number_of_iteration_in_degree_based_annotations
 
 
         inputt=SimpleNamespace(**input)
         good_anchors=find_commnon_MNN(inputt)
         degree_based_annotation(inputt,good_anchors)
 
     return 0
 
 #main()
 
 def degree_based_annotation(input,good_anchors):
     chosenKNN=input.KNN
 
-    resolutionClusterWise=[]
-    for k in range(len(input.resolutionWiseClustering)):
-        sp_leiden_barcode2cluid={}
-        sp_leiden_cluid2barcode={}
-        resolutionwise_spatial_barcode_id=input.resolutionWiseClustering[k]
-        #print('ankit',resolutionwise_spatial_barcode_id[0:5])
-        for i in range(len(resolutionwise_spatial_barcode_id)):
-            id=resolutionwise_spatial_barcode_id[i,1]
-            name=resolutionwise_spatial_barcode_id[i,0]
-            sp_leiden_barcode2cluid[name]=id
-            '''
-            if id not in sp_leiden_cluid2barcode:
-                sp_leiden_cluid2barcode[id]=[name]
-            else:
-                sp_leiden_cluid2barcode[id].append(name)
-            '''
-        resolutionClusterWise.append(sp_leiden_barcode2cluid)
 
+    sp_leiden_barcode2cluid={}
+    sp_leiden_cluid2barcode={}
+    for i in range(len(input.annotation_spatial_barcode_id)):
+            id=input.annotation_spatial_cluster_id[i]
+            name=input.annotation_spatial_barcode_id[i]
+            sp_leiden_barcode2cluid[name]=id
+    resolutionClusterWise=[sp_leiden_barcode2cluid]
 
     deg,G=read_KNN_file(input.KNNfilename)
-
     df=pd.read_csv(input.fname,header=None)
     mnn=df.to_numpy()
 
-    print("all mnn",mnn.shape)
+    #print("all mnn",mnn.shape)
 
     index=[]
     for i in range(len(mnn)):
         name=mnn[i,0]+'#'+mnn[i,1]
         if name in good_anchors:
             index.append(i)
     mnn=mnn[index,:]
 
-    print("good mnn",mnn.shape)
+    #print("good mnn",mnn.shape)
 
     sc_ctype_id=input.lsc[1]
     sc_ctype_name=input.lsc[0]
 
 
     a=np.reshape(input.annotation_singlecell_barcode_id,(len(input.annotation_singlecell_barcode_id),1))
     b=np.reshape(input.annotation_singlecell_cluster_id,(len(input.annotation_singlecell_cluster_id),1))
@@ -705,38 +714,37 @@
                 t2.append(a[j][0])
             confused[key]=t2
             #print(key,t1,t2)
         all_mapped[key]=name[5:]
         #fw.write(key+'\t'+str(name)+'\n')
 
 
-    print('unique mapped 1',len(unique_mapped))
+    #print('unique mapped 1',len(unique_mapped))
     fw=open(input.savepath+'unique_mapped.dat','w')
     for key in unique_mapped:
         fw.write(key+'\t'+'0\n')
     fw.close()
 
     ad_sp= input.ad_sp
     cellname=ad_sp.obs_names.to_numpy()
     genename=ad_sp.var_names.to_numpy()
-    #print(cellname[0:5],genename[0:5])
 
 
     saveunique_mapped=unique_mapped
 
     for res in range(len(resolutionClusterWise)):
         unique_mapped=saveunique_mapped
         all_anchored_mapped=resolved_confused_and_unmapped_mapping_of_cells_deg(confused,G,all_mapped,unique_mapped,[resolutionClusterWise[res]])
-        print('unique mapped 2',len(all_anchored_mapped))
+        #print('unique mapped 2',len(all_anchored_mapped))
         availabled_anchors_mapped=all_anchored_mapped
 
         for iter in range(input.number_of_iteration_in_degree_based_annotations):
             unmapped_cellname,unmapped_deg=find_unmapped_cells_and_deg(deg,availabled_anchors_mapped)
             unique_mapped=resolved_confused_and_unmapped_mapping_of_cells_deg(unmapped_cellname,G,availabled_anchors_mapped,availabled_anchors_mapped,[resolutionClusterWise[res]])
-            print('iter',iter,len(unique_mapped),len(unmapped_cellname),len(unmapped_deg))
+            #print('iter',iter,len(unique_mapped),len(unmapped_cellname),len(unmapped_deg))
 
 
             for i in range(len(cellname)):
                 key=cellname[i]
                 if key not in unique_mapped:
                     unique_mapped[key]='NotMapped'
```

### Comparing `nico_sc_sp-0.0.2/nico/Spatial_Covariations.py` & `nico-sc-sp-0.0.3/nico/Spatial_Covariations.py`

 * *Files 9% similar despite different names*

```diff
@@ -109,124 +109,107 @@
     spatialcell_unique_clusterid=data[:,0]
     CTname=spatialcell_unique_clustername
     CTid=spatialcell_unique_clusterid
 
     df=pd.read_csv(clusterFilename)
     louvainFull=df.to_numpy()
 
-    #for i in range(len(CTname)):
-    #    print(CTname[i],CTid[i])
 
     celltype={}
     cellsinCT={}
     index=[]
     for i in range(len(louvainFull)):
-        #print(louvainFull[i],louvainFull[i][0])
         clu_id=louvainFull[i][1]
         cel_id=louvainFull[i][0]
         if clu_id in CTid:
             index.append(i)
             #celltype[cel_id]=clu_id
             if clu_id not in cellsinCT:
                 cellsinCT[clu_id]=[cel_id]
             else:
                 cellsinCT[clu_id].append(cel_id)
 
     louvain=louvainFull[index,:]
     annotation_spatial_barcode_id= louvain[:,0]
     annotation_spatial_cluster_id= louvain[:,1]
 
-    #print(spatialcell_unique_clustername,spatialcell_unique_clusterid)
     d={}
     for i in range(len(spatialcell_unique_clustername)):
         d[spatialcell_unique_clusterid[i]]=spatialcell_unique_clustername[i]
     annotation_spatial_celltypename=[]
     for i in range(len(annotation_spatial_cluster_id)):
         annotation_spatial_celltypename.append(d[annotation_spatial_cluster_id[i]])
     annotation_spatial_celltypename=np.array(annotation_spatial_celltypename)
 
     return annotation_spatial_celltypename,annotation_spatial_barcode_id,annotation_spatial_cluster_id,spatialcell_unique_clustername,spatialcell_unique_clusterid
 
 
 def find_correlation_bw_genes_and_PC_component_in_singlecell(KcomponentCluster,clusterExpression):
     mat=np.zeros((clusterExpression.shape[1],KcomponentCluster.shape[1]),dtype=float)
-    #print('ankit',KcomponentCluster.shape,clusterExpression.shape,mat.shape)
     for i in range(clusterExpression.shape[1]):
         v1=clusterExpression[:,i]
         for j in range(KcomponentCluster.shape[1]):
             v2=KcomponentCluster[:,j]
             #corr,_ = pearsonr(v1,v2)
             corr,_ =spearmanr(v1,v2)
             #corr=np.corrcoef(v1,v2)
-            #print(corr,corr1)
             mat[i,j]=corr
 
     # mat shape is (# of genes x # of pc) it is a correlation between (PC and genes) of the single cell cluster
     # KcomponentCluster shape is (# of single cell in a single cell cluster x # of pc)
     # clusterExpression shape is (# of single cell in a single cell cluster x # of genes)
-    #print(mat.shape)
     mat=np.nan_to_num(mat)
     return mat
 
 
 def top_genes_in_correlation_list_abs(genename,corr_NMFfactors_genes,n_top_words):
         top_genes_assoc_factors=[]
         for topic_idx, topic in enumerate(abs(corr_NMFfactors_genes.T)):
             top_features_ind = topic.argsort()[: -n_top_words - 1 : -1]
-            #print(topic_idx,sorted(topic))
-            #print(top_features_ind,topic[top_features_ind[0:5]])
             for i in top_features_ind:
                 if i not in top_genes_assoc_factors:
                     top_genes_assoc_factors.append(i)
-        #print(top_genes_assoc_factors)
         gname=genename[top_genes_assoc_factors]
         mat=corr_NMFfactors_genes[top_genes_assoc_factors,:]
         return gname,mat
 
 def top_genes_in_correlation_list_without(genename,corr_NMFfactors_genes,n_top_words):
         top_genes_assoc_factors=[]
         for topic_idx, topic in enumerate(corr_NMFfactors_genes.T):
             top_features_ind = topic.argsort()[: -n_top_words - 1 : -1]
-            #print(topic_idx,sorted(topic))
-            #print(top_features_ind,topic[top_features_ind[0:5]])
             for i in top_features_ind:
                 if i not in top_genes_assoc_factors:
                     top_genes_assoc_factors.append(i)
-        #print(top_genes_assoc_factors)
         gname=genename[top_genes_assoc_factors]
         mat=corr_NMFfactors_genes[top_genes_assoc_factors,:]
 
         return gname,mat
 
 
 def alignment_score(H,spH,ind_H,ind_spH):
-    #print('alignemnt',H.shape,spH.shape,len(ind_H),len(ind_spH))
     r1=H[:,ind_H]
     r2=spH[:,ind_spH]
     comb=np.hstack((r1,r2)).T
     n=len(ind_H)
     knn=max([2,np.ceil(0.01*n) ])
     n_jobs=-1
     k_d,k_ind = cKDTree(comb).query(x=comb, k=knn, workers=n_jobs)
-    #print(n,knn,comb.shape,k_d.shape,k_ind.shape)
 
     avgc1=0
     for i in range(n):
         neigh=k_ind[i]
         c1=0
         for j in range(len(neigh)):
             if neigh[j]<n:
                 c1=c1+1
         avgc1=avgc1+c1
-        #print(i,neigh,len(neigh),c1,c2)
     avgc1=avgc1/n
     #doi:10.1038/nbt.4096
     score=1 - ((avgc1 - (knn/n) ) / (knn - (knn/n) ))
 
-    #print(avgc1,score)
     return score
 
 def multiplicative_method(W,H,A,max_iter):
     norms = []
     e = 1.0e-10
     for n in range(max_iter):
         # Update H
@@ -243,16 +226,15 @@
         #        W[i, j] = W[i, j] * AH_T[i, j] / WHH_T[i, j]
 
         norm = np.linalg.norm(A - W@H, 'fro')
         norms.append(norm)
     return W ,H ,norms
 
 
-def find_PC_of_invidualCluster_in_SC(scbarcode,scadata,no_of_pc,spbarcode,spadata, sct_ad_sc_full,outputdir,celltype_name,threshold_for_LR_exp_in_cell_population):
-    print('\n\n\n')
+def find_PC_of_invidualCluster_in_SC(scbarcode,iNMFmode,NOG_Fa,scadata,no_of_pc,spbarcode,spadata, sct_ad_sc_full,outputdir,celltype_name,cutoff_to_count_exp_cell_population):
 
     #full transcriptome single cell
     cellname=sct_ad_sc_full.obs_names.to_numpy()
     d={}
     for i in range(len(cellname)):
         d[cellname[i]]=i
     index=[]
@@ -308,19 +290,17 @@
     else:
         msp=sct_ad_sp.X
 
     #replace nan to zero
     #msp=np.nan_to_num(msp)
     #msc=np.nan_to_num(msc)
 
-    #print('norm1',np.sum(msc),np.sum(msp),np.sum(CbyG))
     #msc=msc/np.sum(msc)
     #msp=msp/np.sum(msp)
     #CbyG=CbyG/np.sum(CbyG)
-    #print('norm2',np.sum(msc),np.sum(msp),np.sum(CbyG))
     genename_joint=sct_ad_sc.var_names.to_numpy()
     genename_full=full_genes_sc.var_names.to_numpy()
     genename_spatial=sct_ad_sp.var_names.to_numpy()
 
 
     #Gene based normalization
     #msc=np.log10(1+msc)
@@ -334,290 +314,207 @@
     v1=np.zeros((msc.shape[0],n),dtype=float)
     v2=np.zeros((msp.shape[0],n),dtype=float)
     for i in range(n):
         v1[:,i]=msc[:,index[i]]/std1[index[i]]
         v2[:,i]=msp[:,index[i]]/std2[index[i]]
     #sum1=np.std(v1,axis=0)
     #sum2=np.std(v2,axis=0)
-    #print('cell norm3',sum1.shape,sum2.shape,sum1[0:10],sum2[0:10])
 
 
-    '''
-    #Cell based normalization
-    v1=msc[:,index]
-    v2=msp[:,index]
-    sum1=np.std(v1,axis=1)
-    sum2=np.std(v2,axis=1)
-    #print('cell norm2',sum1.shape,sum2.shape,sum1[0:10],sum2[0:10])
-    v1=(v1.T/sum1).T
-    v2=(v2.T/sum2).T
-    sum1=np.std(v1,axis=1)
-    sum2=np.std(v2,axis=1)
-    print('cell norm3',sum1.shape,sum2.shape,sum1[0:10],sum2[0:10])
-    '''
-
-    print('nan v1 v2',np.sum(np.isnan(v1)), np.sum(np.isnan(v2)), np.sum(np.isnan(msp)))
     datasets=[v1,v2]
 
     n1=msc.shape[0]
     n2=msp.shape[0]
     threshold=0.001
     old_score=1
-    for alpha in range(0,51,2):
-    #for alpha in [0]:
-        arr1=[*range(n1)]
-        arr2=[*range(n2)]
-        if n1>n2:
-            np.random.shuffle(arr1)
-            arr1=arr1[0:n2]
-        else:
-            np.random.shuffle(arr2)
-            arr2=arr2[0:n1]
 
-        H,spH,W,V,spV = iNMF(datasets,no_of_pc,value_lambda=alpha,print_obj=False)
+    if iNMFmode==True:
+        for alpha in range(0,51,2):
+            arr1=[*range(n1)]
+            arr2=[*range(n2)]
+            if n1>n2:
+                np.random.shuffle(arr1)
+                arr1=arr1[0:n2]
+            else:
+                np.random.shuffle(arr2)
+                arr2=arr2[0:n1]
+
+            H,spH,W,V,spV = iNMF(datasets,no_of_pc,value_lambda=alpha,print_obj=False)
+            spW=W
+            score=alignment_score(H,spH,arr1,arr2)
+            if abs(score-old_score)<threshold:
+                break
+            old_score=score
+    else:
+        alpha=0
+        model = NMF(n_components=no_of_pc, init = "nndsvda", random_state=1,beta_loss="kullback-leibler",solver="mu",max_iter=1000,alpha_W=0.0,alpha_H=0.0,l1_ratio=0)
+        W = model.fit_transform(v1.T)
+        H = model.components_
         spW=W
+        spH=np.ones((no_of_pc,v2.shape[0]),dtype=float)
+        spW ,spH ,norms=multiplicative_method(spW,spH,v2.T,200)
 
-        #model = NMF(n_components=no_of_pc, init = "nndsvda", random_state=1,beta_loss="kullback-leibler",solver="mu",max_iter=1000,alpha_W=0.0,alpha_H=0.0,l1_ratio=0)
-        #W = model.fit_transform(v1.T)
-        #H = model.components_
-        #spW=W
-        #spH=np.ones((no_of_pc,v2.shape[0]),dtype=float)
-        #spW ,spH ,norms=multiplicative_method(spW,spH,v2.T,200)
 
+    entropy_H=''
+    entropy_SH=''
+    entvalue=[]
 
-        score=alignment_score(H,spH,arr1,arr2)
-        print("alpha",alpha,score)
-        if abs(score-old_score)<threshold:
-            break
-        old_score=score
+    xlabels=[]
+    for i in range(no_of_pc):
+        xlabels.append('NMF'+str(i+1))
+        value=entropy(H[i,:],base=2)  /  np.log2(len(H[i]))
+        entvalue.append(value)
+
+    entvalue=np.array(entvalue)
+    index=np.argsort(-entvalue)
+
+    H=H[index]
+    spH=spH[index]
+
+    for i in range(no_of_pc):
+        entropy_H+=',%0.2f'%(entropy(H[i,:],base=2)  /  np.log2(len(H[i])))
+        entropy_SH+=',%0.2f'%(entropy(spH[i,:],base=2) / np.log2(len(spH[i]))  )
 
 
     #value1=np.sqrt(np.sum((v1.T-np.matmul(W+V,H))**2))
     #value2=np.sqrt(np.sum((v2.T-np.matmul(spW+spV,spH))**2))
-    #print('msc,msp,H,sphH,W,value1,value2,finalAlpha',alpha,msc.shape,msp.shape,H.shape,spH.shape,W.shape,value1,value2)
-
 
-    print('nan',np.sum(np.isnan(spH)), np.sum(np.isnan(spW)), np.sum(np.isnan(msp)))
-    print("SW",len(np.sum(spW,axis=0)), len(np.sum(spW,axis=1)),     np.sum(spW,axis=0),   np.sum(spW,axis=1)[0:5]         )
-    print("SH",len(np.sum(spH,axis=0)), len(np.sum(spH,axis=1)),     np.sum(spH,axis=1),   np.sum(spH,axis=0)[0:5]         )
 
     corr_NMFfactors_genes1=find_correlation_bw_genes_and_PC_component_in_singlecell(H.T,msc)
-    gname1a,geneNMF1a=top_genes_in_correlation_list_abs(genename_joint,corr_NMFfactors_genes1,10)
+    #gname1a,geneNMF1a=top_genes_in_correlation_list_abs(genename_joint,corr_NMFfactors_genes1,10)
     gname1b,geneNMF1b=top_genes_in_correlation_list_without(genename_joint,corr_NMFfactors_genes1,10)
 
     corr_NMFfactors_genes2=find_correlation_bw_genes_and_PC_component_in_singlecell(spH.T,msp)
-    gname2a,geneNMF2a=top_genes_in_correlation_list_abs(genename_spatial,corr_NMFfactors_genes2,10)
+    #gname2a,geneNMF2a=top_genes_in_correlation_list_abs(genename_spatial,corr_NMFfactors_genes2,10)
     gname2b,geneNMF2b=top_genes_in_correlation_list_without(genename_spatial,corr_NMFfactors_genes2,10)
 
     corr_NMFfactors_genes3=find_correlation_bw_genes_and_PC_component_in_singlecell(H.T,CbyG)
-    gname3a,geneNMF3a=top_genes_in_correlation_list_abs(genename_full,corr_NMFfactors_genes3,30)
-    gname3b,geneNMF3b=top_genes_in_correlation_list_without(genename_full,corr_NMFfactors_genes3,30)
+    #gname3a,geneNMF3a=top_genes_in_correlation_list_abs(genename_full,corr_NMFfactors_genes3,30)
+    gname3b,geneNMF3b=top_genes_in_correlation_list_without(genename_full,corr_NMFfactors_genes3,NOG_Fa)
 
 
 
     #df1=pd.DataFrame(W)
     #df1.to_csv(outputdir+celltype_name+'_W.dat',index=False,header=None,float_format='%.5f')
     #df2=pd.DataFrame(spW)
     #df2.to_csv(outputdir+celltype_name+'_spW.dat',index=False,header=None,float_format='%.5f')
     #df3=pd.DataFrame(H.T)
     #df3.to_csv(outputdir+celltype_name+'_H.dat',index=False,header=None,float_format='%.5f')
     #df4=pd.DataFrame(spH.T)
     #df4.to_csv(outputdir+celltype_name+'_spH.dat',index=False,header=None,float_format='%.5f')
 
-    xlabels=[]
-    for i in range(no_of_pc):
-        xlabels.append('NMF'+str(i+1))
 
-    '''
-    fig=plt.figure(figsize=(12,8))
-    gs = fig.add_gridspec(ncols=3, nrows=1, wspace=0.5,width_ratios=[1, 1,2])
-    ax0=fig.add_subplot(gs[0])
-    ax1=fig.add_subplot(gs[1])
-    ax2=fig.add_subplot(gs[2])
-    b=snn.heatmap(geneNMF1a,yticklabels=gname1a,ax=ax0)#componentlabel,ax=ax
-    b.set_xticklabels(xlabels,size = 8,rotation=90)
-    b.set_title('common gene seq data' )
-    b=snn.heatmap(geneNMF2a,yticklabels=gname2a,ax=ax1)#componentlabel,ax=ax
-    b.set_xticklabels(xlabels,size = 8,rotation=90)
-    b.set_title('common gene spatial data')
-    #b.set_yticklabels(b.get_ymajorticklabels(), fontsize = 6)
-
-    fw=open(outputdir+'/'+celltype_name+'_genes_and_correlation.dat','w')
-    for i in range(len(genename_full)):
-        fw.write(genename_full[i]+'\t'+str(corr_NMFfactors_genes3[i])+'\n')
-    fw.close()
-    b=snn.heatmap(geneNMF3a,yticklabels=gname3a,ax=ax2)#componentlabel,ax=ax
-    b.set_xticklabels(xlabels,size = 8,rotation=90)
-    b.set_yticklabels(b.get_ymajorticklabels(), fontsize = 6)
-    b.set_title(celltype_name+', alpha = '+ str(alpha))
-    fig.savefig(outputdir+celltype_name+'_absolute.png',dpi=300)
-    plt.close('all')
-    '''
 
     sc_cluster_mean_exp=np.mean(CbyG,axis=0)
-    sc_cluster_exp_more_than_threshold=CbyG>threshold_for_LR_exp_in_cell_population
+    sc_cluster_exp_more_than_threshold=CbyG>cutoff_to_count_exp_cell_population
     sc_cluster_exp_more_than_threshold=np.sum(sc_cluster_exp_more_than_threshold,axis=0)
     sc_cluster_exp_more_than_threshold=sc_cluster_exp_more_than_threshold/CbyG.shape[0]
 
     selectedGenesAvgExp=np.zeros( (len(gname3b),1) )
     for i in range(len(gname3b)):
         ind=np.where(genename_full==gname3b[i])
         selectedGenesAvgExp[i,0]=np.log10(sc_cluster_mean_exp[ind[0]])
 
-    fig=plt.figure(figsize=(13,8))
+    fig=plt.figure(figsize=(15,10))
     gs = fig.add_gridspec(ncols=4, nrows=1, wspace=0.5,width_ratios=[1, 1,2,0.5])
     ax0=fig.add_subplot(gs[0])
     ax1=fig.add_subplot(gs[1])
     ax2=fig.add_subplot(gs[2])
     ax3=fig.add_subplot(gs[3])
     b=snn.heatmap(geneNMF1b,yticklabels=gname1b,ax=ax0)#componentlabel,ax=ax
     b.set_xticklabels(xlabels,size = 8,rotation=90)
-    b.set_title('common gene seq data' )
+    #b.set_title('common gene seq data' )
+    b.set_title('seq'+entropy_H )
     b=snn.heatmap(geneNMF2b,yticklabels=gname2b,ax=ax1)#componentlabel,ax=ax
     b.set_xticklabels(xlabels,size = 8,rotation=90)
-    b.set_title('common gene spatial data')
+    #b.set_title('common gene spatial data')
+    b.set_title('spatial'+entropy_SH)
     b=snn.heatmap(geneNMF3b,yticklabels=gname3b,ax=ax2)#componentlabel,ax=ax
     b.set_xticklabels(xlabels,size = 8,rotation=90)
     b.set_yticklabels(b.get_ymajorticklabels(), fontsize = 6)
     b.set_title(celltype_name+', alpha = '+ str(alpha))
 
     b=snn.heatmap(selectedGenesAvgExp,yticklabels=gname3b,ax=ax3)#componentlabel,ax=ax
     #b.set_xticklabels('exp',size = 8,rotation=90)
     b.set_yticklabels(b.get_ymajorticklabels(), fontsize = 6)
     b.set_title('log(avg exp)')
-    plt.tight_layout()
-    fig.savefig(outputdir+celltype_name+'_without_absolute.png',dpi=300)
-    plt.close('all')
-
-    '''
-    fig, ax = plt.subplots(9,3,figsize=(10,15))
-    print("pavi",gname,CbyG.shape,H.shape)
-    #pavi ['Dnase1l3' 'Selenop' 'Kdr' 'Vwf' 'Cst3' 'Ctsh' 'Serpina3k' 'Alb' 'Apoa1'] (2706, 24857) (3, 2706)
-    for i in range(len(genename_full)):
-        for j in range(len(gname)):
-            if gname[j]==genename_full[i]:
-                ax[j,0].plot(H[0,:],CbyG[:,i],'.')
-                ax[j,1].plot(H[1,:],CbyG[:,i],'.')
-                ax[j,2].plot(H[2,:],CbyG[:,i],'.')
-
-
-                ax[j,0].set_ylabel(gname[j])
-                ax[j,0].set_title('corr='+str(geneNMF[j,0]))
-                ax[j,1].set_title('corr='+str(geneNMF[j,1]))
-                ax[j,2].set_title('corr='+str(geneNMF[j,2]))
-
-    ax[8,0].set_xlabel('Fa1 H')
-    ax[8,1].set_xlabel('Fa2 H')
-    ax[8,2].set_xlabel('Fa3 H')
-
-    plt.tight_layout()
-    fig.savefig(outputdir+celltype_name+'_correlation.png',dpi=300)
+    #plt.tight_layout()
+    fig.savefig(outputdir+celltype_name+'.png',bbox_inches='tight',transparent=True,dpi=300)
     plt.close('all')
-    '''
 
 
-    #sc_com_pc=W
-    #transfer_sp_com = np.matmul(msp, sc_com_pc)
-    #transfer_sc_com = np.matmul(msc, sc_com_pc)
     transfer_sp_com=spH.T
-    print('\n\n',celltype_name,msc.shape,msp.shape,"W",W.shape,"H",H.shape,'shape','tsp',transfer_sp_com.shape)
-
-
-
-
-
     M=corr_NMFfactors_genes3
     transfer_sc_com=[]
 
 
     sc_barcode=sct_ad_sc.obs_names.to_numpy()
     sp_barcode=sct_ad_sp.obs_names.to_numpy()
     sc_genenames=full_genes_sc.var_names.to_numpy()
 
 
-
-    #print('a1b1',np.std(transfer_sp_com,axis=0))
     #maximum norm or infinity norm normalization
     for i in range(transfer_sp_com.shape[1]):
         #transfer_sp_com[:,i]=transfer_sp_com[:,i]/max(abs(transfer_sp_com[i:,]))
         #l2norm=np.linalg.norm(transfer_sp_com[:,i],ord=2)
         l2norm=np.std(transfer_sp_com[:,i])
         #l1norm=np.linalg.norm(transfer_sp_com[:,i],ord=1)
         #transfer_sp_com[:,i]=transfer_sp_com[:,i]/l1norm
         transfer_sp_com[:,i]=transfer_sp_com[:,i]/l2norm
-        #print(i,transfer_sp_com[:,i],transfer_sp_com[:,i]**2,l1norm,l2norm)
-
-    print('a1b2',np.std(transfer_sp_com,axis=0))
 
 
     return transfer_sp_com, transfer_sc_com, sp_barcode,sc_barcode, M,sc_genenames, sc_cluster_mean_exp,sc_cluster_exp_more_than_threshold
 
 
 
 def makePCneighboorhoodFeatureMatrix(input):
-    #print('xyz',input.annotation_spatial_barcode_id.shape)
     n=len(input.spatialcell_unique_clusterid)
     M=np.zeros((len(input.neighbors),n*input.no_of_pc),dtype=float)
 
-    #fname='spatial_ct_ct_interactions_PC2/save_neighbors_distances.p'
-    #fname='spatial_ct_ct_interactions_Final/save_neighbors_distances.p'
-    #dist_neighbors=pickle.load( open(fname, "rb" ) )
     dist_neighbors=input.neigh_distances
-    print('sss',len(input.neighbors),len(dist_neighbors))
     avgdistArray=0
     for i in range(len(dist_neighbors)):
         avgdistArray=avgdistArray+np.mean(dist_neighbors[i])
     avgdist=avgdistArray/len(dist_neighbors)
 
-    #nd=input.neigh_distances
-    #for i in range(len(nd)):
-    #    print(nd[i],dist_neighbors[i])
 
     for j in range(len(input.neighbors)):
-        #print(j,neighbors[j])
         CC_barcode_id=input.annotation_spatial_barcode_id[j]
         CC_cluster_id=input.annotation_spatial_cluster_id[j]
         PC_component_of_CC=input.pc_of_sp_clusterid[CC_barcode_id]
         PC_component_of_CC=PC_component_of_CC.reshape((1,input.no_of_pc))
         if j==0:
             target=PC_component_of_CC
         else:
             target=np.vstack((target,PC_component_of_CC))
-        #print(target.shape)
 
         neigh_dist=np.array(dist_neighbors[j])
-        #print(neigh_dist,avgdist)
         #weightdist=weightdist/avgdist
         neigh_dist=1/neigh_dist
         sum_weight_dist=np.sum(neigh_dist)
         weighted_avg_dist=neigh_dist/sum_weight_dist
-        #print(j,len(input.neighbors[j]),neigh_dist,sum_weight_dist,weighted_avg_dist)
         temp={}
         for k in range(len(input.neighbors[j])):
             id=input.neighbors[j][k]
             NC_barcode_id=input.annotation_spatial_barcode_id[id]
             NC_cluster_id=input.annotation_spatial_cluster_id[id]
             PC_component_of_NC=input.pc_of_sp_clusterid[NC_barcode_id]
             PC_component_of_NC=PC_component_of_NC.reshape((1,input.no_of_pc))
             factor=weighted_avg_dist[k]
             if NC_cluster_id not in temp:
                 temp[NC_cluster_id]=factor*PC_component_of_NC
-                #print(temp[NC_cluster_id].shape)
             else:
                 temp[NC_cluster_id]=np.concatenate((temp[NC_cluster_id],factor*PC_component_of_NC))
-                #print(len(neighbors[j]),NC_cluster_id,temp[NC_cluster_id].shape)
-            #print(PC_component_of_NC)
 
         for key in input.spatialcell_unique_clusterid:
             start_index=input.no_of_pc*key
             end_index=start_index+input.no_of_pc
             if key in temp:
                 M[j,start_index:end_index]=np.sum(temp[key],axis=0)
-        #print(j,temp)
-            #d[NC_barcode_id]=1
+
 
     #cluster=input.annotation_spatial_cluster_id
     #cluster=cluster.reshape((len(cluster),1))
     #df=pd.DataFrame(np.hstack((cluster,M)))
     df=pd.DataFrame(np.hstack((target,M)))
     df.to_csv(input.outputname,index=True,header=None)
 
@@ -648,35 +545,25 @@
         PCA_of_sc_cluster_accordingto_spatial_clusterid={}
         for i in range(n):
             clidsp=input.spatialcell_unique_clusterid[i]
             index=np.where(input.annotation_spatial_cluster_id==clidsp)
             spbarcode=input.annotation_spatial_barcode_id[index[0]]
             scbarcode=[]
             for j in range(len(input.singlecell_unique_clustername)):
-                #print(input.singlecell_unique_clustername[j],input.spatialcell_unique_clustername[i])
                 if input.singlecell_unique_clustername[j]==input.spatialcell_unique_clustername[i]:
                     clid=input.singlecell_unique_clusterid[j]
                     index=np.where(input.annotation_singlecell_cluster_id==clid)
                     scbarcode=input.annotation_singlecell_barcode_id[index[0]]
                     break
 
-            pc_sp,pc_sc,sp_barcode,sc_barcode,sc_HVG_correlation,sc_genenames,sc_cluster_mean_exp,sc_cluster_exp_more_than_threshold=find_PC_of_invidualCluster_in_SC(scbarcode,input.ad_sc,input.no_of_pc,spbarcode,input.ad_sp, sct_ad_sc_full, input.nmf_output,input.spatialcell_unique_clustername[i],input.threshold_for_LR_exp_in_cell_population)
-            #for kkkk in range(len(sc_genenames)):
-            #    if sc_genenames[kkkk]=='Mptx2':
-            #        print('ankit',sc_cluster_mean_exp[kkkk])
-
-            #check orthogonality
-            #print("1 spatial orthogonality",sum(pc_sp[:,0]*pc_sp[:,1]) )
-            #print("1 SC orthogonality",sum(pc_sc[:,0]*pc_sc[:,1]) )
+            pc_sp,pc_sc,sp_barcode,sc_barcode,sc_HVG_correlation,sc_genenames,sc_cluster_mean_exp,sc_cluster_exp_more_than_threshold=find_PC_of_invidualCluster_in_SC(scbarcode,input.iNMFmode,input.NOG_Fa,input.ad_sc,input.no_of_pc,spbarcode,input.ad_sp, sct_ad_sc_full, input.nmf_output,input.spatialcell_unique_clustername[i],input.cutoff_to_count_exp_cell_population)
 
-            print(i,input.spatialcell_unique_clustername[i],pc_sp.shape,sc_HVG_correlation.shape,sc_genenames.shape)
             PCA_of_sc_cluster_accordingto_spatial_clusterid[clidsp]=[sc_HVG_correlation,pc_sp,sc_genenames,sc_cluster_mean_exp,sc_cluster_exp_more_than_threshold]
             for k in range(len(sp_barcode)):
                 pc_of_sp_clusterid[sp_barcode[k]]=pc_sp[k]
-            #pc_of_sp_clusterid[input.spatialcell_unique_clusterid[i]]=pc_sp
 
     return pc_of_sp_clusterid,PCA_of_sc_cluster_accordingto_spatial_clusterid
 
 
 
 def model_linear_regression(input,savedir,logistic_predicted_interactions):
     shap_cluster_cutoff=input.shap_cluster_cutoff
@@ -684,41 +571,36 @@
     #ind=~np.isnan(data1).any(axis=1)
     #data=data1[ind,:]
     data=np.nan_to_num(data1)
 
     featureVector=range(input.no_of_pc+1,data.shape[1]) # #just neighborhood
     AllneighborhoodClass= data[:,featureVector]
     Alltarget= data[:,1:input.no_of_pc+1]
-    #print(AllneighborhoodClass.shape,Alltarget.shape)
 
     count=0
     for i in range(len(input.spatialcell_unique_clusterid)):
         temp=np.where(input.spatialcell_unique_clusterid[i]==input.annotation_spatial_cluster_id)
         index=temp[0]
         neighborhoodClass=AllneighborhoodClass[index,:]
         target=Alltarget[index,:]
         positive_interacted_CT= logistic_predicted_interactions[input.spatialcell_unique_clustername[i]]
-        #print(i,neighborhoodClass.shape,target.shape,input.spatialcell_unique_clustername[i])
-        #print(positive_interacted_CT)
         newindex=[]
         xlabel=[]
         score=[]
         for j in range(len(input.spatialcell_unique_clustername)):
             start=j*input.no_of_pc
             end=start+input.no_of_pc
             for k in range(len(positive_interacted_CT)):
                 if positive_interacted_CT[k][0]==input.spatialcell_unique_clustername[j]:
-                    #print(i,start,end)
                     xlabel.append(positive_interacted_CT[k][0])
                     score.append(positive_interacted_CT[k][1])
                     for kk in range(start,end):
                         newindex.append(kk)
 
         neighborhoodClass=neighborhoodClass[:,newindex]
-        #print("\n\n\n\n",i,neighborhoodClass.shape,target.shape)
         xlabel=np.array(xlabel)
         score=np.array(score)
 
         ylabelname=[]
         for k in range(len(xlabel)):
             for j in range(input.no_of_pc):
                 ylabelname.append(xlabel[k]+'_s'+'%0.3f'%score[k]+'_Fa'+str(j+1))
@@ -727,38 +609,35 @@
         saveoutname=str(input.spatialcell_unique_clusterid[i])+'_'+input.spatialcell_unique_clustername[i]
         coef,intercept,alpha,percent_variance_explained,residual_variance_explained,pv=run_ridge_regression(input,savedir,saveoutname,ylabelname,target,neighborhoodClass,shap_cluster_cutoff)
         #coef_mu,comp_score,coef_std,comp_score_std,alpha=run_ridge_regression(input.seed ,input.lambda_c,input.K_fold,input.n_repeats,target,neighborhoodClass)
         savedata=savedir+'coef'+str(input.spatialcell_unique_clusterid[i])+'.npz'
         np.savez(savedata,coef_mu=coef,intercept=intercept,alpha=alpha,xlabel=xlabel,score=score,Yreg=target,Xreg=neighborhoodClass,pvalue=pv,pve=percent_variance_explained,rve=residual_variance_explained)
         #np.savez(savedata,coef_mu=coef_mu,coef_std=coef_std,comp_score=comp_score,comp_score_std=comp_score_std,alpha=alpha,xlabel=xlabel,score=score)
 
-
-    print(count)
+    #print(count)
 
 
 
 
 
 def run_ridge_regression(input,savedir,saveoutname,ylabelname,target,neighborhoodClass,shap_cluster_cutoff):
     seed=input.seed+1
 
     train_index=range(target.shape[0])
     test_index=[]
     x_train,x_test=neighborhoodClass[train_index],neighborhoodClass[test_index]
     y_train,y_test=target[train_index],target[test_index]
 
-    create_directory(savedir+'plot_Y_and_X/')
-
-    if input.shap_computation:
+    #create_directory(savedir+'plot_Y_and_X/')
+    if input.shap_analysis:
         dir1=savedir+'Shapley_Interventional/'
         dir2=savedir+'Shapley_FullConventional/'
         create_directory(dir1)
         create_directory(dir2)
 
-    print("std dev",np.std(y_train,axis=0))
     LRI=[]
     LRC=[]
     yhat=[]
     lambda_c=[]
     Xdata=x_train
     for i in range(y_train.shape[1]):
         linear_model = RidgeCV(alphas=input.lambda_c)
@@ -766,32 +645,29 @@
         pipe=Pipeline([('ridge_regression',linear_model)])
         pipe.fit(Xdata,y_train[:,i])
         yyhat=pipe.predict(Xdata)
         yhat.append(yyhat)
         LR= pipe.named_steps['ridge_regression']
         coef=LR.coef_
         intercept=LR.intercept_
-        #print(LR.alpha_, LR.lambda_, LR.scores_[-1],coef,intercept)
         LRI.append(intercept)
         LRC.append(coef)
         lambda_c.append('%0.2f'%LR.alpha_)
 
     LRI=np.array(LRI)
     yhat=np.array(yhat).T
     LRC=np.array(LRC)
 
 
     #mu=np.mean(y_train,axis=0)
     #total_ss= np.sum((y_train-mu)**2,axis=0)
     #residual_ss=np.sum((y_train-yhat)**2,axis=0)
     #explained_ss= np.sum((yhat-mu)**2,axis=0)
-    #print(explained_ss+residual_ss, total_ss)
     #percent_variance_explained=100*explained_ss/total_ss
     #residual_variance_explained=100*residual_ss/total_ss
-    #print(saveoutname,percent_variance_explained,residual_variance_explained,lambda_c)
 
     pv=np.ones(LRC.shape,dtype=float)
     EVS=[]
     rss=[]
     for i in range(y_train.shape[1]):
                 #EVS.append(explained_variance_score(save_y_test[:,i], save_y_pred[:,i]))
                 EVS.append(explained_variance_score(y_train[:,i], yhat[:,i]))
@@ -812,36 +688,31 @@
                         else:
                             raise
                     sd_b = np.sqrt(var_b)
                     ts_b = params/ sd_b
                     df = x_train.shape[0] - x_train.shape[1]
                     p_values1 =np.array([[2*(1-scipy.stats.t.cdf(np.abs(ii),df-1)) for ii in ts_b]])
                     pv[i]=p_values1[:,1:]
-                    if flag==1:
-                        print(i,saveoutname,MSE,"var_b",var_b,"pvalue",pv[i])
+                    #if flag==1:
+                    #    print(i,saveoutname,MSE,"var_b",var_b,"pvalue",pv[i])
+
 
-                #print("\ntrain ",i,Xdata.shape,y_train.shape)
-                #print('Coef=',LRC[i])
-                #print('Intercept=',LRI)
-                #print('MSE=',MSE,', sd_b=',sd_b, ', ts_b=', ts_b,  '\tpv=',pv[i])
 
         #print("LRC",LRC.shape,LRI.shape)
         #x_train2 = sm.add_constant(Xdata)
         #est1=sm.OLS(y_train[:,0],x_train2).fit()
         #print("summary1",est1.summary())
         #est2=sm.OLS(y_train[:,1],x_train2).fit()
         #print("summary2",est2.summary())
         #est3=sm.OLS(y_train[:,2],x_train2).fit()
         #print("summary3",est3.summary())
 
 
     if False:#(saveoutname=='12_LSECs')|(saveoutname=='11_KCs')|(saveoutname=='20_Stellate_cells'):
-
-            print(saveoutname,yname[0],rss,residual_ss,explained_ss)
-
+            #print(saveoutname,yname[0],rss,residual_ss,explained_ss)
             fw=open(savedir+'plot_Y_and_X/'+saveoutname+'_'+yname[0]+'_.dat','w')
             for i in range(Xdata.shape[0]):
                 fw.write(str(y_train[i,0])+','+str(y_train[i,1])+','+str(y_train[i,2])+','+str(Xdata[i,0])+','+str(Xdata[i,1])+','+str(Xdata[i,2])+'\n')
             fw.close()
 
             fig, ax = plt.subplots(3,3,figsize=(10,8))
             ax[0,0].plot(Xdata[:,0],y_train[:,0],'b.')
@@ -863,41 +734,40 @@
             ax[0,0].set_ylabel(saveoutname+'_Fa1')
             ax[1,0].set_ylabel(saveoutname+'_Fa2')
             ax[2,0].set_ylabel(saveoutname+'_Fa3')
 
             for i in range(len(LRC)):
                 for j in range(len(LRC[i])):
                     ax[i,j].set_title('C=%0.3f'%LRC[i,j]+',I=%0.3f'%LRI[i]+',pv=%0.3f'%pv[i,j]+', lamda='+str(lambda_c),fontsize=8)
-            plt.tight_layout()
-            fig.savefig(savedir+'plot_Y_and_X/'+saveoutname+'_'+yname[0]+'_.png',dpi=300, bbox_inches = "tight")
+            #plt.tight_layout()
+            fig.savefig(savedir+'plot_Y_and_X/'+saveoutname+'_'+yname[0]+'_.png',dpi=300, transparent=True,bbox_inches = "tight")
             plt.close('all')
 
 
-    if input.shap_computation:
+    if input.shap_analysis:
             #explainer = shap.LinearExplainer(LR, x_train)
             explainer = shap.explainers.Linear(LR, x_train,feature_names=ylabelname,feature_perturbation="interventional")
             #explainer = shap.Explainer(LR, x_train,feature_names=ylabelname)
             #shap_values = explainer.shap_values(x_train)
             shap_values = explainer(x_train)
 
-            #shap.waterfall_plot(explainer.expected_value, shap_values[sample_ind], X.iloc[sample_ind], max_display=14)
-            clust = shap.utils.hclust(x_train, y_train, linkage="single")
-            shap.plots.bar(shap_values, clustering=clust, clustering_cutoff=shap_cluster_cutoff, show=False)
-            plt.title("True to the model")
-            plt.tight_layout()
-            plt.savefig(dir1+saveoutname+'_.png',dpi=300, bbox_inches = "tight")
-            plt.close('all')
-
-            explainer = shap.explainers.Linear(LR, x_train,feature_names=ylabelname,feature_perturbation="correlation_dependent")
-            shap_values = explainer(x_train)
-            shap.plots.bar(shap_values, clustering=clust, clustering_cutoff=shap_cluster_cutoff, show=False)
-            plt.title("True to the data")
-            plt.tight_layout()
-            plt.savefig(dir2+saveoutname+'_.png',dpi=300, bbox_inches = "tight")
-            plt.close('all')
+            for i in range(y_train.shape[1]):
+                #shap.waterfall_plot(explainer.expected_value, shap_values[sample_ind], X.iloc[sample_ind], max_display=14)
+                clust = shap.utils.hclust(x_train, y_train[:,i], linkage="single")
+                shap.plots.bar(shap_values, clustering=clust, clustering_cutoff=shap_cluster_cutoff, show=False)
+                plt.title("True to the model "+saveoutname+'_'+'Fa'+str(i+1)+", EVS = " +'%0.4f'%EVS[i])
+                plt.savefig(dir1+saveoutname+'_Fa'+str(i+1)+'.png',dpi=300, bbox_inches = "tight")
+                plt.close('all')
+
+                explainer = shap.explainers.Linear(LR, x_train,feature_names=ylabelname,feature_perturbation="correlation_dependent")
+                shap_values = explainer(x_train)
+                shap.plots.bar(shap_values, clustering=clust, clustering_cutoff=shap_cluster_cutoff, show=False)
+                plt.title("True to the data "+saveoutname+'_'+'Fa'+str(i+1)+", EVS = " +'%0.4f'%EVS[i])
+                plt.savefig(dir2+saveoutname+'_Fa'+str(i+1)+'.png',dpi=300, bbox_inches = "tight")
+                plt.close('all')
 
     coef=LRC
     intercept=LRI
     residual_variance_explained=0
 
     return coef,intercept,lambda_c,EVS,residual_variance_explained,pv
 
@@ -930,24 +800,22 @@
                     if j!=(len(l)-1):
                         temp+='--'
                 if meanCoefficients[ highestIndex[i]]>logistic_coef_cutoff:
                     positiveprediction.append(temp)
                     score.append(meanCoefficients[ highestIndex[i]])
                 else:
                     negativeprediction.append(temp)
-            #print(predictedCT,len(score))
             InteractingCTs.append([predictedCT,positiveprediction, score   ])
 
     logistic_predicted_interactions={}
     for i in range(len(InteractingCTs)):
         cCT=InteractingCTs[i][0]
         nCT=InteractingCTs[i][1]
         Interacting_score=InteractingCTs[i][2]
         for j in range(len(nCT)):
-            #print(i,j,cCT,nCT[j],Interacting_score[j],)
             if cCT not in logistic_predicted_interactions:
                 logistic_predicted_interactions[cCT]=[[nCT[j],Interacting_score[j]]]
             else:
                 logistic_predicted_interactions[cCT].append([nCT[j],Interacting_score[j]])
 
     return logistic_predicted_interactions
 
@@ -976,15 +844,15 @@
         colorbar.set_ticklabels(['pv>=0.05', 'pv<0.05'])
 
     return b
 
 
 
 def plot_results(savedir,maindir,radius,input):
-
+    RegFigSize=input.RegFigSize
     for i in range(len(input.spatialcell_unique_clusterid)):
         filename=input.spatialcell_unique_clustername[i]
         temp=np.where(input.spatialcell_unique_clusterid[i]==input.annotation_spatial_cluster_id)
         index=temp[0]
         savedata=savedir+'coef'+str(input.spatialcell_unique_clusterid[i])+'.npz'
         data=np.load(savedata,allow_pickle=True)
         coef_mu=data['coef_mu']
@@ -1001,15 +869,14 @@
         xlabel=data['xlabel']
         score=data['score']
 
         componentlabel=[]
         for j in range(input.no_of_pc):
             componentlabel.append('Fa'+str(j+1))
 
-        #print(pve,rve)
         percentVE=''
         percentRE=''
 
         for j in range(len(pve)):
             if j!=0:
                 percentVE+=', '
                 percentRE+=', '
@@ -1024,47 +891,40 @@
 
         #tempG=pvalue<0.1
         #m1,m2=tempG.nonzero()
         #coef_mu[m1,m2]=0
         #coef_mu=tempG.astype(int)
 
         #pvalue=pvalue<0.05
-        #print('11',filename,pvalue)
         pvalue[pvalue<10**-10]=10**-10
         pvalue=-np.log10(pvalue)
         pvalue=np.nan_to_num(pvalue)
-        #pvalue[pvalue == np.inf] = 100
-        #print('22','\n33',np.max(pvalue))
 
-        #print('\n\n\n')
-        # significant pvalue is 1  less than 0.05
-        #print("anki",coef_mu.shape,rve.shape,pvalue.shape)
 
 
-        fig, ax = plt.subplots(1,1,figsize=(10,3.5))
+        fig, ax = plt.subplots(1,1,figsize=RegFigSize)
         M=pvalue.shape[1]
         N=pvalue.shape[0]
         c=coef_mu
         x, y = np.meshgrid(np.arange(M), np.arange(N))
         R = pvalue/10.0/2
         maxp=pvalue.max()
-        print(filename,maxp)
         circles = [plt.Circle((j,i), radius=r) for r, j, i in zip(R.flat, x.flat, y.flat)]
         col = PatchCollection(circles, array=c.flatten(), cmap='jet')#cmap="RdYlGn")
         ax.add_collection(col)
         ax.set(xticks=np.arange(M), yticks=np.arange(N),
                xticklabels=ylabelname, yticklabels=componentlabel)
         ax.set_xticks(np.arange(M+1)-0.5, minor=True)
         ax.set_yticks(np.arange(N+1)-0.5, minor=True)
         ax.set_xticklabels(ylabelname,size = 8,rotation=90)
         ax.set_title(filename+r',$\alpha$='+str(alpha)+',EVS='+percentVE,fontsize=6)
         ax.grid(which='minor')
         fig.colorbar(col)
-        fig.tight_layout()
-        fig.savefig(savedir+'11coeff_matrix_'+str(input.spatialcell_unique_clusterid[i])+'_'+filename+'.png',dpi=300)
+        #fig.tight_layout()
+        fig.savefig(savedir+'pvalue_significance_coeff_matrix_'+str(input.spatialcell_unique_clusterid[i])+'_'+filename+'.png',bbox_inches='tight',transparent=True,dpi=300)
         plt.close('all')
 
 
 
         fig=plt.figure(figsize=(10,5))
         gs = fig.add_gridspec(ncols=1, nrows=2, height_ratios=[3, 1])
         ax0=fig.add_subplot(gs[0])
@@ -1081,23 +941,24 @@
 
         b=snn.heatmap(pvalue,cmap=snn.cm.rocket_r,yticklabels=componentlabel,ax=ax1)
         #colorbar=b.collections[0].colorbar
         #b=chooseRightColorBarForPvalue(ax1,pvalue,componentlabel)
         b.xaxis.tick_top()
         xlabels= b.get_xticks()
         b.set_xticklabels(xlabels,size = 0)
+        b.set_yticklabels(componentlabel,rotation = 0)
         #b.axes.get_xaxis().set_visible(False)
         #b.set_ylabel('Principal components')
         #_, ylabels= plt.yticks()
         #b.set_yticklabels(ylabels, size = 5)
         #plt.title(filename+r',$\alpha$='+str(alpha)+',VE='+percentVE+',RE='+percentRE)
         #b.set_title('pvalue significant ')
 
         fig.tight_layout()
-        fig.savefig(savedir+'coeff_matrix_'+str(input.spatialcell_unique_clusterid[i])+'_'+filename+'.png',dpi=300)
+        fig.savefig(savedir+'coeff_matrix_'+str(input.spatialcell_unique_clusterid[i])+'_'+filename+'.png',bbox_inches='tight',transparent=True,dpi=300)
         plt.close('all')
 
 
     ylabelname=[]
     for i in range(len(input.spatialcell_unique_clustername)):
         for j in range(input.no_of_pc):
             ylabelname.append(input.spatialcell_unique_clustername[i]+'_'+'Fa'+str(j+1))
@@ -1105,60 +966,92 @@
 
     fig,axs=plt.subplots(1,1,figsize=(10,10))
     name=maindir+'Principal_component_feature_matrix'+str(input.no_of_pc)+'.csv'
     data=np.genfromtxt(open(name, "rb"), delimiter=',', skip_header=0)
     Feature=data[:,(1+input.no_of_pc):data.shape[1]]
     index=np.argsort(input.annotation_spatial_cluster_id)
     snn.heatmap(np.log10(Feature[index,:]),xticklabels=ylabelname)
-    fig.tight_layout()
-    fig.savefig(maindir+'Feature_matrix_PC'+str(input.no_of_pc)+'.png',dpi=300)
+    #fig.tight_layout()
+    fig.savefig(maindir+'Feature_matrix_PC'+str(input.no_of_pc)+'.png',bbox_inches='tight',transparent=True,dpi=300)
     fig.clf()
 
 
-def main(myinput):
-    celltypefname=myinput.celltypefname
-    clusterfname=myinput.clusterfname
-    sct_ad_sp=myinput.ad_sp
-    sct_ad_sc=myinput.ad_sc
-    full_ad_sc=myinput.full_ad_sc
-    input_spatial_analysis_dir=myinput.input_spatial_analysis_dir
-    inputRadius=myinput.inputRadius
-    no_of_pc=myinput.no_of_pc
-    strategy=myinput.strategy
-    maindir1=myinput.outdir
-    gene_set_names=myinput.gene_set_names
-    database=myinput.database
-    pathwayorganism=myinput.pathwayorganism
-    pathwayCutoff=myinput.pathwayCutoff
-    shap_cluster_cutoff=myinput.shap_cluster_cutoff
-    LRdb=myinput.LRdb
-    pathway_plot=myinput.pathway_plot
-    coeff_cutoff_for_rid_reg=myinput.coeff_cutoff_for_rid_reg
-    seed=myinput.seed
-    lambda_c=myinput.lambda_c
-    K_fold=myinput.K_fold
-    n_repeats=myinput.n_repeats
-    n_jobs=myinput.n_jobs
-    shap_computation=myinput.shap_computation
-    logistic_coef_cutoff=myinput.logistic_coef_cutoff
-    gene_correlation_plots_and_sheets=myinput.gene_correlation_plots_and_sheets
-    pvalueCutoff=myinput.pvalueCutoff
-
-    threshold_for_LR_exp_in_cell_population=myinput.threshold_for_LR_exp_in_cell_population
-    plotting_threshold_for_cell_pop_LR=myinput.plotting_threshold_for_cell_pop_LR
-    plotting_threshold_for_NMF_factors_LR=myinput.plotting_threshold_for_NMF_factors_LR
+def gene_covariation_analysis(ref_cluster_file,ref_CTname_file,outputdir='./spatial_ct_ct_interactions/',
+ref_common_genes_h5ad='./inputSC/common_counts_sc.h5ad',
+ref_full_genes_h5ad='./inputSC/Original_counts.h5ad',
+que_common_genes_h5ad='./inputSP/common_counts_sp.h5ad',delimiter=',',
+LRdbFilename='./LR_db_omnipath_highConfidence.txt',iNMFmode=True,no_of_pc=3,seed=3685134,Radius=0,pvalueCutoff=0.05,gene_correlation_in_excel_sheets=True,
+shap_analysis=False,shap_cluster_cutoff=0.5,cutoff_to_count_exp_cell_population=0,LR_plot_NMF_Fa_thres=0.5,LR_plot_Exp_thres=0.5,
+pathway_plot=False,pathwayCutoff=0.5,pathwayorganism='Mouse',lambda_c=list(np.power(2.0, np.arange(-10, 10))),
+database=['BioPlanet_2019','Reactome_2016'],coeff_cutoff_for_rid_reg=0,logistic_coef_cutoff=0,NOG_Fa=30,
+RegFigSize=(10,1.25),LRFigSize=(15, 11)):
+
+
+    '''
+    Default parameters are following:
+
+    There should be no header information in cell type filename (ref_CTname_file)
+    The cluster filenaname (ref_cluster_file) should have the header information
+    The output annotation file will be saved in outputdir/Regression_R_*
+
+    ref_cluster_file #give a scRNAseq cluster file
+    ref_CTname_file #give a scRNAseq cluster cell type name (first column is cluster id, and second column is cell type name)
+    outputdir='./spatial_ct_ct_interactions/'
+
+    ref_common_genes_h5ad='./inputSC/'common_counts_sc.h5ad'  #input common gene scRNAseq count data in h5ad format
+    ref_full_genes_h5ad='./inputSC/Original_counts.h5ad' #input full gene scRNAseq count data in h5ad format
+    que_common_genes_h5ad='./inputSP/common_counts_sp.h5ad' #input common gene spatial count data in h5ad format
+    delimiter=',' #This delimiter used in the ref_CTname_file
+
+    LRdbFilename='./LR_db_omnipath_highConfidence.txt' #is the filename of ligand receptor database (first column is ligand and second column is receptor)
+    iNMFmode=True #By default it will compute integrated NMF If it is false then the analysis performs the basic NMF
+    no_of_pc=3 #number of factors used in NMF
+    seed=3685134
+    Radius=0  #This radius parameter should be same as used in spatial_neighborhood_analysis
+    pvalueCutoff=0.05 #cutoff use in the ridge regression steps to find the significant factor-celltype vs factor-celltype interactions
+    gene_correlation_in_excel_sheets=True #True show the gene correlation with the factors in the excel sheet, If false then it would not show
+    shap_analysis=False  #If it is true then it perform the shap analysis
+    shap_cluster_cutoff=0.5  #Shap analysis parameter
+    cutoff_to_count_exp_cell_population=0    #This is used to find how many cells expressed a given gene in a given cell type. Value 0 is Fine with count data
+    LR_plot_NMF_Fa_thres=0.5  #Ligand Receptor plot use factor cutoff to find the enriched LR pairs
+    LR_plot_Exp_thres=0.5 #Ligand Receptor plot use % expressed cell population cutoff to find the enriched LR pairs
+    pathway_plot=False  #If true then pathway figures will generate using gseapy package
+    pathwayCutoff=0.5   #gseapy parameter to find the pathway enriched library from the top 100 gene list from each factor of a given cell type
+    pathwayorganism='Mouse' #Organism used in the gseapy package
+    database=['BioPlanet_2019','Reactome_2016'] #database used in the gseapy pathway
+
+    lambda_c=list(np.power(2.0, np.arange(-10, 10)))  #regularization parameter use in the ridge regression step
+    coeff_cutoff_for_rid_reg=0 #this cutoff is use for to make the list of significant celltype_factor-celltype_factor interactions whose absolute regression coefficient is greater than this
+    logistic_coef_cutoff=0 #this cutoff is use to know the niche interactions (cell type -cell type interactions) When it is >0 then cell type - cell type likely to interact with each other
+    NOG_Fa=30 #number of genes use in each factor to show the NMF plots "./spatial_ct_ct_interactions/Regression_R_*/NMF_output"
+    RegFigSize=(10,1.25) #width and height of the figure in "./spatial_ct_ct_interactions/Regression_R_*/Regression_outputs*"
+    LRFigSize=(15, 11) #width and height of the figure in "./spatial_ct_ct_interactions/Regression_R_*/Plot_ligand_receptor_in_interacting_celltypes/*"
+
+    '''
+
+
 
+    f=open(LRdbFilename,'r')
+    LRdb=f.readlines()
+    f.close()
+
+    sct_ad_sp=sc.read_h5ad(que_common_genes_h5ad)
+    sct_ad_sc=sc.read_h5ad(ref_common_genes_h5ad)
+    full_ad_sc=sc.read_h5ad(ref_full_genes_h5ad)
+    maindir1=outputdir+'Regression_R_'
 
+    strategy='L2_multi'+'_linear/'  #myinput.strategy
+    gene_set_names=[]
 
-    df=pd.read_csv(clusterfname)
+    df=pd.read_csv(ref_cluster_file )
     data=df.to_numpy()
     annotation_singlecell_barcode_id=data[:,0]
     annotation_singlecell_cluster_id=data[:,1]
 
-    with open(celltypefname,'r') as f:
+    with open(ref_CTname_file,'r') as f:
         cont = f.read()
         lines=cont.split('\n')
         singlecell_unique_clustername=[]
         singlecell_unique_clusterid=[]
         for i in range(len(lines)):
             l=lines[i].split('\t')
             if len(l)>1:
@@ -1180,54 +1073,50 @@
 
     annotation_singlecell_celltypename=[]
     for i in range(len(annotation_singlecell_cluster_id)):
         annotation_singlecell_celltypename.append(d[annotation_singlecell_cluster_id[i]])
     annotation_singlecell_celltypename=np.array(annotation_singlecell_celltypename)
 
 
-    print('sc1 annotation_singlecell_cluster_id',len(annotation_singlecell_cluster_id))
-    print('sc2 annotation_singlecell_barcode_id',len(annotation_singlecell_barcode_id))
-    print('sc3 annotation_singlecell_celltypename',len(annotation_singlecell_celltypename))
-    print('sc4 singlecell_unique_clustername', len(singlecell_unique_clustername))
+    #print('sc1 annotation_singlecell_cluster_id',len(annotation_singlecell_cluster_id))
+    #print('sc2 annotation_singlecell_barcode_id',len(annotation_singlecell_barcode_id))
+    #print('sc3 annotation_singlecell_celltypename',len(annotation_singlecell_celltypename))
+    #print('sc4 singlecell_unique_clustername', len(singlecell_unique_clustername))
 
 
     # load spatial dat
 
     sp_genename=sct_ad_sp.var_names.to_numpy()
     sc_genename=sct_ad_sc.var_names.to_numpy()
     index_sp,index_sc=find_index(sp_genename,sc_genename)
     print('common genes between sc and sp',len(index_sp),len(index_sc))
     ad_sp_ori=sct_ad_sp[:,index_sp].copy()
     ad_sc_ori=sct_ad_sc[:,index_sc].copy()
 
 
-
+    inputRadius=[Radius]
     for radius in inputRadius:
-        celltypeFilename=input_spatial_analysis_dir+'BiologicalNameOfCT.dat'
-        clusterFilename=input_spatial_analysis_dir+'save_clusterid_'+str(radius)+'.csv'
+        celltypeFilename=outputdir+'BiologicalNameOfCT.dat'
+        clusterFilename=outputdir+'save_clusterid_'+str(radius)+'.csv'
 
         annotation_spatial_celltypename,annotation_spatial_barcode_id,annotation_spatial_cluster_id,spatialcell_unique_clustername,spatialcell_unique_clusterid=read_spatial_data(clusterFilename,celltypeFilename)
 
-        print('\nsp1 annotation_spatial_cluster_id',len(annotation_spatial_cluster_id))
-        print('sp2 annotation_spatial_barcode_id',len(annotation_spatial_barcode_id))
-        print('sp3 annotation_spatial_celltypename',len(annotation_spatial_celltypename))
-        print('sp4 spatialcell_unique_clustername', len(spatialcell_unique_clustername))
 
-        neighbors=pickle.load( open(input_spatial_analysis_dir+'save_neighbors_'+str(radius)+'.p', "rb" ) )
-        distances=pickle.load( open(input_spatial_analysis_dir+'save_distances_'+str(radius)+'.p', "rb" ) )
+        neighbors=pickle.load( open(outputdir+'save_neighbors_'+str(radius)+'.p', "rb" ) )
+        distances=pickle.load( open(outputdir+'save_distances_'+str(radius)+'.p', "rb" ) )
 
         maindir=maindir1+str(radius)+'/'
         create_directory(maindir)
         outputname=maindir+'Principal_component_feature_matrix'+str(no_of_pc)+'.csv'
         inputdata={}
         inputdata['no_of_pc']=no_of_pc
         inputdata['outputname']=outputname
 
 
-        fname=input_spatial_analysis_dir+strategy+'/save_numpy_array_'+str(radius)+'.npz'
+        fname=outputdir+strategy+'/save_numpy_array_'+str(radius)+'.npz'
         data=np.load(fname,allow_pickle=True)
         logistic_coef=data['coef']
         logistic_cmn=data['cmn']
         logistic_cmn_std=data['cmn_std']
         logistic_coef_std=data['coef_std']
         logistic_CTFeatures=data['CTFeatures']
         #f=open(input_spatial+'BiologicalNameOfCT.dat')
@@ -1235,17 +1124,14 @@
         nameOfCellType={}
         for line in f:
             l=line[0:-1].split('\t')
             nameOfCellType[int(l[0])]=l[1]
 
         logistic_predicted_interactions=find_logistic_regression_interacting_score(logistic_cmn,logistic_coef,logistic_CTFeatures,nameOfCellType,logistic_coef_cutoff)
 
-        #for key in logistic_predicted_interactions:
-        #    print(key,logistic_predicted_interactions[key])
-
 
 
         inputdata['ad_sp']=ad_sp_ori #sct_ad_sp
         inputdata['ad_sc']=ad_sc_ori#sct_ad_sc#
         inputdata['annotation_spatial_cluster_id']=annotation_spatial_cluster_id
         inputdata['annotation_spatial_barcode_id']=annotation_spatial_barcode_id
         inputdata['annotation_spatial_celltypename']=annotation_spatial_celltypename
@@ -1259,99 +1145,105 @@
         inputdata['singlecell_unique_clusterid']=singlecell_unique_clusterid
         inputdata['neighbors']=neighbors
         inputdata['neigh_distances']=distances
         create_directory(maindir+'NMF_output/')
         inputdata['nmf_output']=maindir+'NMF_output/'
         inputdata['seed']=seed
         inputdata['lambda_c']=lambda_c
-        inputdata['K_fold']=K_fold
-        inputdata['n_repeats']=n_repeats
-        inputdata['n_jobs']=n_jobs
-        inputdata['shap_computation']=shap_computation
+        inputdata['iNMFmode']=iNMFmode
+        #inputdata['K_fold']=K_fold
+        #inputdata['n_repeats']=n_repeats
+        #inputdata['n_jobs']=n_jobs
+        inputdata['shap_analysis']=shap_analysis
         inputdata['shap_cluster_cutoff']=shap_cluster_cutoff
 
         inputdata['logistic_coef_cutoff']=logistic_coef_cutoff
         inputdata['coeff_cutoff_for_rid_reg']=coeff_cutoff_for_rid_reg
         inputdata['gene_set_names']=gene_set_names
         inputdata['database']=database
         inputdata['pathwayorganism']=pathwayorganism
         inputdata['pathwayCutoff']=pathwayCutoff
         inputdata['pathway_plot']=pathway_plot
         inputdata['pvalueCutoff']=pvalueCutoff
-
-        inputdata['threshold_for_LR_exp_in_cell_population']=threshold_for_LR_exp_in_cell_population
-        inputdata['plotting_threshold_for_cell_pop_LR']=plotting_threshold_for_cell_pop_LR
-        inputdata['plotting_threshold_for_NMF_factors_LR']=plotting_threshold_for_NMF_factors_LR
+        inputdata['NOG_Fa']=NOG_Fa
+        inputdata['LRFigSize']=LRFigSize
+        inputdata['RegFigSize']=RegFigSize
+
+        inputdata['cutoff_to_count_exp_cell_population']=cutoff_to_count_exp_cell_population
+        inputdata['LR_plot_Exp_thres']=LR_plot_Exp_thres
+        inputdata['LR_plot_NMF_Fa_thres']=LR_plot_NMF_Fa_thres
 
         input=SimpleNamespace(**inputdata)
 
         flag=1
         if os.path.isfile(outputname):
             filesize = os.path.getsize(outputname)
             if filesize>0: #If file is already exist and have size greater than 0 then no need to run again. It will save some time if you want to run it again with different parameters
                 flag=0
 
         if flag==1:
-            #print(sct_ad_sc)
             pc_of_sp_clusterid,PCA_of_sc_cluster_accordingto_spatial_clusterid=compute_PC_space(input,full_ad_sc)
             # full_ad_sc use in only find_PC_of_invidualCluster_in_SC function
             # ideally it should be sctransform way of normalized matrix equivalent to sct_ad_sc but
             # if not then need to do perform scaling HVG etc
             pickle.dump(PCA_of_sc_cluster_accordingto_spatial_clusterid,open(maindir+'PCA_of_sc_cluster'+str(no_of_pc)+'.p', 'wb'))
             inputdata['pc_of_sp_clusterid']=pc_of_sp_clusterid
             input=SimpleNamespace(**inputdata)
             #Principal_component_feature_matrix5.csv saving in this function
             makePCneighboorhoodFeatureMatrix(input)
 
         savedir=maindir+'/Regression_outputs'+str(no_of_pc)+'/'
         create_directory(savedir)
         existornot=savedir+'coef'+str(input.spatialcell_unique_clusterid[-1])+'.npz'
         if os.path.isfile(existornot):
-            pass
-            #plot_results(savedir,maindir,radius,input)
+            #pass
+            plot_results(savedir,maindir,radius,input)
         else:
             model_linear_regression(input,savedir,logistic_predicted_interactions)
             plot_results(savedir,maindir,radius,input)
 
+        print("Regression step done")
+
         totalLRpairs=read_LigRecDb(LRdb)
         find_canonical_pathways_in_interacting_cell_types(input,maindir,savedir,totalLRpairs)
+        print("ligand receptors step done")
 
-        if gene_correlation_plots_and_sheets:
+        if gene_correlation_in_excel_sheets:
             made_excel_sheet_for_gene_correlation(maindir,input)
+            print("gene correlation in excel sheets step done")
 
         if input.pathway_plot:
             savename=maindir+'/Pathway_figures/'
             create_directory(savename)
             pathway_analysis(input,maindir,savename)#top_genes_in_CC,CC_gene,CC_meanExpression)
+            print("pathway step done")
 
 
 
 
 def pathway_analysis(input,maindir,savename):#background_geneName,background_expression
 
     database=input.database
     pathwayorganism=input.pathwayorganism
     pathwayCutoff=input.pathwayCutoff
-    coeff_cutoff_for_log_reg=input.logistic_coef_cutoff
-    coeff_cutoff_for_rid_reg=input.coeff_cutoff_for_rid_reg
-    gene_set_names=input.gene_set_names
-    pvalueCutoff=input.pvalueCutoff
-    LRcutoff=input.plotting_threshold_for_NMF_factors_LR
-    plotting_threshold_for_cell_pop_LR=input.plotting_threshold_for_cell_pop_LR
+    #coeff_cutoff_for_log_reg=input.logistic_coef_cutoff
+    #coeff_cutoff_for_rid_reg=input.coeff_cutoff_for_rid_reg
+    #gene_set_names=input.gene_set_names
+    #pvalueCutoff=input.pvalueCutoff
+    LR_plot_Exp_thres=input.LR_plot_Exp_thres
     nog=100
 
     PCA_of_sc_cluster_accordingto_spatial_clusterid=pickle.load(open(maindir+'PCA_of_sc_cluster'+str(input.no_of_pc)+'.p', 'rb'))
     n=len(input.spatialcell_unique_clustername)
 
 
 
     for fi in range(n):
         clid=input.spatialcell_unique_clusterid[fi]
         Factors,CC_PCA,CC_gene,CC_meanExpression,CC_popExpression=PCA_of_sc_cluster_accordingto_spatial_clusterid[clid]
-        #print(input.spatialcell_unique_clustername[i],gene[0:10],gene[-10:-1])
         CC_celltype_name=input.spatialcell_unique_clustername[fi]
 
         for j in range(input.no_of_pc):
             source=Factors[:,j]
             ind=np.argsort(-source)
             interestofGene=[]
             value=[]
@@ -1361,52 +1253,48 @@
                     interestofGene.append(CC_gene[ind[k]])
                     value.append(source[ind[k]])
 
             if len(interestofGene)>nog:
                 va1=value[0:nog]
                 ga1=interestofGene[0:nog]
                 cutoff=va1[-1]
-                #print(max(va1),min(va1))
             else:
                 ga1=interestofGene
                 va1=value
 
-            #print(source[ind[0:5]])
-            print(fi,j+1,Factors.shape,CC_celltype_name,ga1[0:2],va1[0:2])
-
             titlename='Fa'+str(j+1)+'_'+CC_celltype_name+'_c'+str(int(100*cutoff))
             for i in range(len(database)):
                 titlename1=titlename+'_'+database[i]
                 finalsavename=savename+titlename1
                 titlename1=titlename1+'_#G='+str(len(ga1))
-                #print("tt",titlename)
-                #print("fin",finalsavename)
+
                 enr_res1 = gseapy.enrichr(gene_list=ga1,organism=pathwayorganism,gene_sets=database[i], description='pathway',cutoff = pathwayCutoff)
                 #enr_res1 = gseapy.enrichr(gene_list=g1,organism='Mouse',gene_sets=background_model,description='pathway',cutoff = 0.5)
                 finalsavename.replace(' ','_')
                 try:
                     gseapy.barplot(enr_res1.res2d,title=titlename1,ofname=finalsavename,fontsize=12)#database[i]+titlename
                 except Exception as e: #Exception: Error getting the Enrichr libraries
                     pass
 
 
 
 
 def find_canonical_pathways_in_interacting_cell_types(input,maindir,savedir,totalLRpairs):
 
-    database=input.database
-    pathwayorganism=input.pathwayorganism
-    pathwayCutoff=input.pathwayCutoff
-    pathway_plot=input.pathway_plot
+    #database=input.database
+    #pathwayorganism=input.pathwayorganism
+    #pathwayCutoff=input.pathwayCutoff
+    #pathway_plot=input.pathway_plot
+    LRFigSize=input.LRFigSize
     coeff_cutoff_for_log_reg=input.logistic_coef_cutoff
     coeff_cutoff_for_rid_reg=input.coeff_cutoff_for_rid_reg
     gene_set_names=input.gene_set_names
     pvalueCutoff=input.pvalueCutoff
-    LRcutoff=input.plotting_threshold_for_NMF_factors_LR
-    plotting_threshold_for_cell_pop_LR=input.plotting_threshold_for_cell_pop_LR
+    LRcutoff=input.LR_plot_NMF_Fa_thres #Used in excel sheet to show the enrichment of ligand receptor intera
+    LR_plot_Exp_thres=input.LR_plot_Exp_thres
 
     PCA_of_sc_cluster_accordingto_spatial_clusterid=pickle.load(open(maindir+'PCA_of_sc_cluster'+str(input.no_of_pc)+'.p', 'rb'))
     n=len(input.spatialcell_unique_clustername)
 
 
     workbook = xlsxwriter.Workbook(maindir+'/Lig_and_Rec_enrichment_in_interacting_celltypes'+str(input.no_of_pc)+'.xlsx')
     fout=open(maindir+'/Regression_summary_'+str(input.no_of_pc)+'.dat','w')
@@ -1425,15 +1313,14 @@
         clid=input.spatialcell_unique_clusterid[i]
         clname=input.spatialcell_unique_clustername[i]
         d[clname]=clid
 
     for i in range(n):
         clid=input.spatialcell_unique_clusterid[i]
         CC_corr,CC_PCA,CC_gene,CC_meanExpression,CC_popExpression=PCA_of_sc_cluster_accordingto_spatial_clusterid[clid]
-        #print(input.spatialcell_unique_clustername[i],gene[0:10],gene[-10:-1])
         CC_celltype_name=input.spatialcell_unique_clustername[i]
         #temp=np.where(input.spatialcell_unique_clusterid[i]==input.annotation_spatial_cluster_id)
         #index=temp[0]
         savedata=savedir+'coef'+str(input.spatialcell_unique_clusterid[i])+'.npz'
         data=np.load(savedata,allow_pickle=True)
         coef_mu=data['coef_mu']
         intercept=data['intercept']
@@ -1494,16 +1381,14 @@
                 if (pvalue[k,j]<pvalueCutoff)&(abs(normalized_ridge_coef[k,j])>coeff_cutoff_for_rid_reg):
                 #if True:
                     if score[index]>coeff_cutoff_for_log_reg:
                         NC_corr,NC_PCA,NC_gene,NC_meanExpression,NC_popExpression=PCA_of_sc_cluster_accordingto_spatial_clusterid[d[NC_celltype_name[index]]]
                         top_genes_in_CC,top_genes_in_NC,genesWithUP,genesWithDown,Found1,Found2=find_fold_change(CC_corr,NC_corr,CC_gene,k,pc_index_nc[j],totalLRpairs,LRcutoff,CC_meanExpression,NC_meanExpression,CC_popExpression,NC_popExpression)
                         common_genes=list(set(top_genes_in_CC).intersection(set(top_genes_in_NC)))
 
-                        print(len(top_genes_in_CC),len(top_genes_in_NC),len(common_genes))
-
                         for ele in range(len(Found1)):
                             header=[str(i)+'-'+str(interaction_id),CC_celltype_name+'(cc)',NC_celltype_name[index]+'(nc)',score[index],k+1,1+pc_index_nc[j],normalized_ridge_coef[k,j] ,'Ligand(A)','Receptor(B)','GeneCor(Lig)','GeneCor(Rec)','Receptor(A)','Ligand(B)','GeneCor(Rec)','GeneCor(Lig)']
                             header[7]=Found1[ele][0][0]
                             header[8]=Found1[ele][1][0]
                             header[9]=Found1[ele][0][1]
                             header[10]=Found1[ele][1][1]
                             header[11]=Found1[ele][0][2]
@@ -1530,19 +1415,19 @@
                             for ri in range(15):
                                 worksheet.write(worksheetrow,ri,header[ri])
                                 worksheet_local.write(worksheetrow_local,ri,header[ri])
                             worksheetrow+=1
                             worksheetrow_local+=1
 
 
-                        plot_ligand_receptor_in_interacting_celltypes(CC_celltype_name,NC_celltype_name[index],score[index],k+1,1+pc_index_nc[j],normalized_ridge_coef[k,j],pvalue[k,j],Found1,Found2,saveLRplots,plotting_threshold_for_cell_pop_LR)
+                        plot_ligand_receptor_in_interacting_celltypes(CC_celltype_name,NC_celltype_name[index],score[index],k+1,1+pc_index_nc[j],normalized_ridge_coef[k,j],pvalue[k,j],Found1,Found2,saveLRplots,LR_plot_Exp_thres,LRFigSize)
 
-                        print('\n\nankit',CC_celltype_name,'CC-Fa'+str(k+1)+'\t'+'%0.3f'%(score[index])+'\tNC-Fa'+str(1+pc_index_nc[j])+'\t'+
-                        NC_celltype_name[index]+'\t%0.3f'%(normalized_ridge_coef[k,j])+'\t'+str(interaction_id))
-                        print('anusha',normalized_ridge_coef.shape, intercept.shape, Xreg[:,j].shape,Yreg[:,k].shape,i,k,j,index,'\t',pc_index_nc[j], CC_PCA.shape, NC_PCA.shape)
+                        #print(CC_celltype_name,'CC-Fa'+str(k+1)+'\t'+'%0.3f'%(score[index])+'\tNC-Fa'+str(1+pc_index_nc[j])+'\t'+
+                        #NC_celltype_name[index]+'\t%0.3f'%(normalized_ridge_coef[k,j])+'\t'+str(interaction_id))
+                        #print(normalized_ridge_coef.shape, intercept.shape, Xreg[:,j].shape,Yreg[:,k].shape,i,k,j,index,'\t',pc_index_nc[j], CC_PCA.shape, NC_PCA.shape)
                         #save_dat_for_checking(maindir,input,Yreg[:,k],Xreg[:,j],CC_corr[:,[k]], NC_corr[:,[pc_index_nc[j]]],CC_gene,CC_celltype_name,str(k+1), NC_celltype_name[index],str(1+pc_index_nc[j]), coef_mu[k,j],normalized_ridge_coef[k,j], intercept[k], str(interaction_id))
                         #print('CC',len(top_genes_in_CC),top_genes_in_CC[0:1],genesWithUP[0:1])
                         #print('NC',len(top_genes_in_NC),top_genes_in_NC[0:1],genesWithDown[0:1])
 
                         if len(genesWithUP)>0:
                             #name_cc='_CC_'+CC_celltype_name.replace('.','_')+'_PC'+str(k+1)#+'_ID'+str(interaction_id)
                             name_cc=CC_celltype_name.replace('.','_')+'_Fa'+str(k+1)#+'_ID'+str(interaction_id)
@@ -1579,15 +1464,14 @@
         r=totalLRpairs[i][1]
         listofallLR[l]=1
         listofallLR[r]=1
         name=l+'--'+r
         if name not in uniqueLRpairs:
             uniqueLRpairs[name]=1
 
-    #print(PCA.shape,NH_PCA.shape)
     first=PCA[:,CCPC]
     second=NH_PCA[:,NCPC]
     ind1=np.argsort(-abs(first))
     ind2=np.argsort(-abs(second))
 
     cc_genes=[]
     cc_genes2=[]
@@ -1684,57 +1568,51 @@
         headersave_full=[]
         headersave_common=[]
         sort_full=[]
         sort_common=[]
         for k in range(input.no_of_pc):
             sort_full.append([])
             sort_common.append([])
-        #print(CC_corr)
         for j in range(len(CC_corr)):
             ind=~np.isnan(CC_corr[j]).any(axis=0)
-            #print(i,ind)
             if ind==True:
                 ax.text(CC_corr[j,0],CC_corr[j,1],gene[j],fontsize=5)
                 header=[gene[j]]
                 for k in range(input.no_of_pc):
                     sort_full[k].append(CC_corr[j,k]) #without absolute
                     header.append(CC_corr[j,k])
                 headersave_full.append(header)
                 if gene[j] in genenames:
                     headersave_common.append(header)
                     for k in range(input.no_of_pc):
                         sort_common[k].append(CC_corr[j,k]) #without absolute
 
 
-        #print(headersave_common)
-
         ax.set_xlabel('PC1')
         ax.set_ylabel('PC2')
         ax.set_title(input.spatialcell_unique_clustername[i])
-        fig.tight_layout()
-        fig.savefig(outputFolder+'correlation_'+input.spatialcell_unique_clustername[i]+'.png',bbox_inches='tight',dpi=300)
+        #fig.tight_layout()
+        fig.savefig(outputFolder+'correlation_'+input.spatialcell_unique_clustername[i]+'.png',bbox_inches='tight',transparent=True,dpi=300)
         plt.close('all')
 
 
         for k in range(input.no_of_pc):
             worksheetrow=fixvalue
             indsort=np.argsort(-np.array(sort_full[k]))
-            #print('ankitankur',input.no_of_pc,len(indsort))
             for rj in range(len(indsort)):
                 header=headersave_full[indsort[rj]]
                 for ri in range(len(header)):
                     worksheetFullGene[k].write(worksheetrow,(input.no_of_pc+2)*i+ri,header[ri])
                 worksheetrow+=1
 
             worksheetrow=fixvalue
             indsort=np.argsort(-np.array(sort_common[k]))
             for rj in range(len(indsort)):
                 header=headersave_common[indsort[rj]]
                 for ri in range(len(header)):
-                    #print("ABC",i,k,rj,ri)
                     worksheetSpatialGene[k].write(worksheetrow,(input.no_of_pc+2)*i+ri,header[ri])
                 worksheetrow+=1
 
     workbook.close()
 
 
 
@@ -1752,54 +1630,26 @@
     trianglesS = [(i + 1 + (j + 1) * (M + 1), i + (j + 1) * (M + 1), cstart + i + j * M)
                   for j in range(N) for i in range(M)]
     trianglesW = [(i + (j + 1) * (M + 1), i + j * (M + 1), cstart + i + j * M)
                   for j in range(N) for i in range(M)]
     return [Triangulation(x, y, triangles) for triangles in [trianglesN, trianglesE, trianglesS, trianglesW]]
 
 
-def  plot_ligand_receptor_in_interacting_celltypes(CC_celltype_name,NC_celltype_name,logRegScore,pc1,pc2,ridgeRegScore,pvalue,Found1,Found2,saveLRplots,plotting_threshold_for_cell_pop_LR):
+def  plot_ligand_receptor_in_interacting_celltypes(CC_celltype_name,NC_celltype_name,logRegScore,pc1,pc2,ridgeRegScore,pvalue,Found1,Found2,saveLRplots,LR_plot_Exp_thres,LRFigSize):
 
     '''
     for i in range(len(data)):
         A.append(AC[i]+'_Fa_'+str(AF[i])+'_'+lig[i])
         B.append(BN[i]+'_Fa_'+str(BF[i])+'_'+rec[i])
     A=np.sort(np.unique(A))
     B=np.sort(np.unique(B))
     ML=np.zeros((len(A), len(B)),dtype=float)
     MR=np.zeros((len(A), len(B)),dtype=float)
 
     '''
-    flag=0
-    if (CC_celltype_name=='cDC2s')&(NC_celltype_name=='Hep145_P'):
-        flag=1
-    if (CC_celltype_name=='Cholangiocytes')&(NC_celltype_name=='Portain_Vein_EC'):
-        flag=1
-    if (CC_celltype_name=='Cholangiocytes')&(NC_celltype_name=='Hep145_P'):
-        flag=1
-    if (CC_celltype_name=='Cholangiocytes')&(NC_celltype_name=='Hep2_MP'):
-        flag=1
-    if (CC_celltype_name=='Hep145_P')&(NC_celltype_name=='LSECs'):
-        flag=1
-    if (CC_celltype_name=='Hep145_P')&(NC_celltype_name=='KCs'):
-        flag=1
-    if (CC_celltype_name=='LSECs')&(NC_celltype_name=='Hep145_P'):
-        flag=1
-    if (CC_celltype_name=='Hep378_MC')&(NC_celltype_name=='LSECs'):
-        flag=1
-
-    if (CC_celltype_name=='Stellate_cells')&(NC_celltype_name=='LSECs'):
-        flag=1
-    if (CC_celltype_name=='T_cells')&(NC_celltype_name=='ILC1s'):
-        flag=1
-    if (CC_celltype_name=='LSECs')&(NC_celltype_name=='Hep378_MC'):
-        flag=1
-    if (CC_celltype_name=='Central_Vein_EC')&(NC_celltype_name=='Stellate_cells'):
-        if (pc1==2)&(pc2==3):
-            flag=1
-
     flag=1
 
     if flag==1:
         ligand=[]
         receptor=[]
         fact_lig=[]
         fact_rec=[]
@@ -1809,85 +1659,42 @@
         B=[]
         for ele in range(len(Found1)):
             #header=['Ligand(A)','Receptor(B)','GeneCor(Lig)','GeneCor(Rec)','Receptor(A)','Ligand(B)','GeneCor(Rec)','GeneCor(Lig)']
             #header[11]=Found1[ele][0][2]
             #header[12]=Found1[ele][1][2]
             ligExpCellPop=Found1[ele][0][3]
             recExpCellPop=Found1[ele][1][3]
-            if ((ligExpCellPop>plotting_threshold_for_cell_pop_LR)&(recExpCellPop>plotting_threshold_for_cell_pop_LR)):
+            if ((ligExpCellPop>LR_plot_Exp_thres)&(recExpCellPop>LR_plot_Exp_thres)):
                 ligand.append(Found1[ele][0][0])
                 receptor.append(Found1[ele][1][0])
                 fact_lig.append(float(Found1[ele][0][1]))
                 fact_rec.append(float(Found1[ele][1][1]))
                 popExp_lig.append(Found1[ele][0][3])
                 popExp_rec.append(Found1[ele][1][3])
                 A.append(CC_celltype_name+'(cc)_Fa'+str(pc1)+'_'+Found1[ele][0][0])
                 B.append(NC_celltype_name+'(nc)_Fa'+str(pc2)+'_'+Found1[ele][1][0])
 
         for ele in range(len(Found2)):
             ligExpCellPop=Found2[ele][0][3]
             recExpCellPop=Found2[ele][1][3]
-            if ((ligExpCellPop>plotting_threshold_for_cell_pop_LR)&(recExpCellPop>plotting_threshold_for_cell_pop_LR)):
+            if ((ligExpCellPop>LR_plot_Exp_thres)&(recExpCellPop>LR_plot_Exp_thres)):
                 ligand.append(Found2[ele][0][0])
                 receptor.append(Found2[ele][1][0])
                 fact_lig.append(float(Found2[ele][0][1]))
                 fact_rec.append(float(Found2[ele][1][1]))
                 popExp_lig.append(Found2[ele][0][3])
                 popExp_rec.append(Found2[ele][1][3])
                 A.append(NC_celltype_name+'(nc)_Fa'+str(pc2)+'_'+Found2[ele][0][0])
                 B.append(CC_celltype_name+'(cc)_Fa'+str(pc1)+'_'+Found2[ele][1][0])
 
-        #print('0',CC_celltype_name+'_Fa'+str(pc1)+'_'+NC_celltype_name+'_Fa'+str(pc2))
-        #print('1',A)
-        #print('2',B)
 
         if (len(A)>0)&(len(B)>0):
             nA=np.sort(np.unique(A))
             nB=np.sort(np.unique(B))
-            print(CC_celltype_name,NC_celltype_name,logRegScore,len(Found1),len(Found2),len(ligand),len(A),len(B),len(nA),len(nB))
-            '''
-            MLF=np.zeros((len(nA), len(nB)),dtype=float) #factor
-            MRF=np.zeros((len(nA), len(nB)),dtype=float)
-            MLE=np.zeros((len(nA), len(nB)),dtype=float) #number of cell population expressed this genes
-            MRE=np.zeros((len(nA), len(nB)),dtype=float)
-            for i in range(len(A)):
-                name1=A[i]
-                name2=B[i]
-                row=0
-                col=0
-                for j in range(len(nA)):
-                    if nA[j]==name1:
-                        row=j
-                for j in range(len(nB)):
-                    if nB[j]==name2:
-                        col=j
-                MLF[row,col]=fact_lig[i]
-                MRF[row,col]=fact_rec[i]
-                MLE[row,col]=popExp_lig[i]
-                MRE[row,col]=popExp_rec[i]
-                #print(row,col,name1,name2,)
-
-            fig=plt.figure(figsize=(25,40))
-            #gs = gridspec.GridSpec(2, 1, width_ratios=[1, 1])
-            ax0=plt.subplot(2,1,1)#    plt.subplot(gs[0])
-            ax1=plt.subplot(2,1,2)#plt.subplot(gs[1])
-            #fig.suptitle('LigRec Plot',fontsize=12)
-            snn.heatmap(ax=ax0,data=MLE,annot=False, fmt='0.2f',     xticklabels=nB, annot_kws={"size": 5},yticklabels=nA)
-            snn.heatmap(ax=ax1,data=MRE,annot=False, fmt='0.2f',     xticklabels=nB, annot_kws={"size": 5},yticklabels=nA)
-            #plt.xlabel('Spatial cell clusters')
-            #plt.ylabel('Single cell clusters')
-
-            pvalue='%0.2f'%(-np.log10(pvalue))
-            ax0.set_title('SpatialScore=%0.3f'%logRegScore+', RidgeRegScore=%0.2f'%ridgeRegScore +', pv='+pvalue  )
-            #g.xaxis.set_ticks_position("top")
-            plt.tight_layout()
-            savefname=CC_celltype_name+'_Fa'+str(pc1)+'_'+NC_celltype_name+'_Fa'+str(pc2)
-            fig.savefig(saveLRplots+savefname+'.png',dpi=300)
-            plt.close('all')
-            '''
+            #print(CC_celltype_name,NC_celltype_name,logRegScore,len(Found1),len(Found2),len(ligand),len(A),len(B),len(nA),len(nB))
 
             #A=np.array(A)
             #B=np.array(B)
             fact_lig=np.array(fact_lig)
             fact_rec=np.array(fact_rec)
             popExp_rec=np.array(popExp_rec)
             popExp_lig=np.array(popExp_lig)
@@ -1912,30 +1719,27 @@
                                'north': fact_lig,
                                'south': fact_rec,
                                'east': popExp_rec,
                                'west':  popExp_lig})
 
             df['rows'] = pd.Categorical(df['rows'],categories=nA)  # fix an ordering,
             df_piv = df.pivot_table(index='rows', columns='cols')
-            #print('\n\n\n\n\n',df_piv)
             M = len(df_piv.columns) // 4
             N = len(df_piv)
 
             values = [df_piv[dir] for dir in ['north', 'east', 'south', 'west']]  # these are the 4 column names in df
 
             triangul = triangulation_for_triheatmap(M, N)
             #cmaps = ['RdYlBu'] * 4
             #cmaps =['cool','copper','cool','copper']
             cmaps =['Blues','copper_r','Blues','copper_r']
             #norms = [plt.Normalize(0, 1) for _ in range(4)]
             norms = [plt.Normalize(fmin, fmax),plt.Normalize(pmin, pmax),plt.Normalize(fmin, fmax),plt.Normalize(pmin, pmax)]
 
-
-            #fig, ax = plt.subplots(figsize=(7.5, 5.5))
-            fig, ax = plt.subplots(figsize=(15, 11))
+            fig, ax = plt.subplots(figsize=LRFigSize)
 
             imgs = [ax.tripcolor(t, np.ravel(val), norm=norm,cmap=cmap,ec='white')  #norm=[]
                     for t, val, cmap, norm in zip(triangul, values, cmaps, norms)]
 
             #ax.tick_params(length=0)
             #ax.set_title('localizationCoef='+'%0.3f'%np.unique(localized)+',regressionCoef='+'%0.3f'%np.unique(regCoff))
             ax.set_xticks(range(M))
@@ -1943,20 +1747,20 @@
             ax.set_yticks(range(N))
             ax.set_yticklabels(df_piv.index)
             ax.invert_yaxis()
             ax.margins(x=0, y=0)
             pvalue='%0.2f'%(-np.log10(pvalue))
             ax.set_title(CC_celltype_name+'_Fa'+str(pc1)+', '+NC_celltype_name+'_Fa'+str(pc2)+', SS=%0.3f'%logRegScore+', RRS=%0.2f'%ridgeRegScore +', pv='+pvalue  )
             #ax.set_aspect('equal', 'box')  # square cells
-            plt.colorbar(imgs[0], ax=ax,label='correlation values in the factors')
+            plt.colorbar(imgs[0], ax=ax,label='correlation value in the factors')
             plt.colorbar(imgs[1], ax=ax,label='%expressed cell population')
 
-            plt.tight_layout()
+            #plt.tight_layout()
             savefname=CC_celltype_name+'_Fa'+str(pc1)+'_'+NC_celltype_name+'_Fa'+str(pc2)
-            fig.savefig(saveLRplots+savefname+'.png',dpi=300)
+            fig.savefig(saveLRplots+savefname+'.png',bbox_inches='tight', transparent=True,dpi=300)
             plt.close('all')
             #'''
 
 
 def read_LigRecDb(contdb):
     #f=open('sort_3_db_L_R_high_confident.dat','r')
     totalLRpairs=[]
@@ -2015,20 +1819,19 @@
 
         #CC_corr=CC_corr.reshape((len(CC_corr),1))
         #NC_corr=NC_corr.reshape((len(NC_corr),1))
         data1=np.hstack((NC_corr,CC_corr))
         ind=~np.isnan(data1).any(axis=1)
         data=data1[ind,:]
         gene=g_cc[ind]
-        #print('pavi',pca_cc.shape,pca_nc.shape,data.shape, gene.shape)
 
         ax[1].scatter(data[:,0],data[:,1],s=1,marker='o',c='b')
         for i in range(len(gene)):
             ax[1].text(data[i,0],data[i,1],gene[i],fontsize=5)
         ax[1].set_xlabel(xname)
 
 
-        fig.tight_layout()
+        #fig.tight_layout()
         #plt.matshow(np.outer(np.sort(model.row_labels_) + 1, np.sort(model.column_labels_) + 1),cmap=plt.cm.Blues)
         #plt.title("Checkerboard structure of rearranged data")
-        fig.savefig(savecorrelation+myname+'.png',dpi=300)
+        fig.savefig(savecorrelation+myname+'.png',bbox_inches='tight',transparent=True,dpi=300)
         plt.close('all')
```

### Comparing `nico_sc_sp-0.0.2/nico/Spatial_Interactions.py` & `nico-sc-sp-0.0.3/nico/Spatial_Interactions.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 import warnings
 import time
 #import pickle5 as pickle
 from scipy.cluster.hierarchy import dendrogram, linkage
 from matplotlib import cm
 from matplotlib.colors import ListedColormap, LinearSegmentedColormap
 import networkx as nx
+import pickle
+import pandas as pd
 
 warnings.filterwarnings('ignore')
 #export PYTHONWARNINGS='ignore:Multiprocessing-backed parallel loops:UserWarning'
 os.environ["PYTHONWARNINGS"] = "ignore::UserWarning"
 
 
 
@@ -774,114 +776,178 @@
 
             fig.tight_layout()
             fig.savefig(filename+'/Rank'+str(k+1)+'_'+nameOfCellType[goodPredictedCellType[k]],bbox_inches='tight',dpi=300)
             fig.clf()
 
 
 
-def run_logistic_regression_on_spatial_features(inputdir,n_repeats,K_fold,coeff_cutoff,strategy,seed,n_jobs,lambda_c_ranges,BothLinearAndCrossTerms,radius,figuresize):
-        f=open(inputdir+'BiologicalNameOfCT.dat')
+def spatial_neighborhood_analysis(outputdir='./spatial_ct_ct_interactions/',
+pos_file='./inputSP/tissue_positions_list.csv',
+cluster_file='./inputSP/MNN_based_annotations/3_deg_annotation_spatial_cluster.csv',
+CTname_file='./inputSP/MNN_based_annotations/3_deg_annotation_spatial_ct_name.dat',Radius=0,n_repeats=1,K_fold=5,seed=36851234,
+n_jobs=-1,lambda_c_ranges=list(np.power(2.0, np.arange(-12, 12))),coeff_cutoff=20,delimiter=',',
+removed_CTs_before_finding_CT_CT_interactions=['NM'],
+figsize=[2.5,2.5], figsize_eval=[4,3],figsize_niche=[10,7],niche_cutoff=0.12):
+
+
+
+        '''
+        Default parameters are following:
+
+        If user wants to run for multiple parameters then it is good practice to change the outputdir name or delete the old one
+        If average neighbor is quite low (<1) then increase the radius and then try to perform neighborhood analysis
+        There should be no header information in position filename (pos_file) and cell type filename (CTname_file)
+        The cluster filenaname (cluster_file) should have the header information
+
+
+        outputdir='./spatial_ct_ct_interactions/'
+        pos_file='./inputSP/tissue_positions_list.csv'
+        cluster_file='./inputSP/MNN_based_annotations/3_deg_annotation_spatial_cluster.csv'
+        CTname_file='./inputSP/MNN_based_annotations/3_deg_annotation_spatial_ct_name.dat'
+        Radius=0 #Radius 0 will perform the delaunay triangulation
+        n_repeats=1 #no of times to run the logistic regression after finding the hyperparameters
+        K_fold=5 #no of cross folds
+        seed=36851234
+        n_jobs=-1 #no of processors For details see here https://scikit-learn.org/stable/glossary.html#term-n_jobs
+        lambda_c_ranges=list(np.power(2.0, np.arange(-12, 12))) # inverse of lambda regularization
+        delimiter=',' #This delimiter used in the CTname_file
+        removed_CTs_before_finding_CT_CT_interactions=['NM'] #this cell type would not be use in the neighborohood analysis
+        figsize=[2.5,2.5]   #width and height of the figures in  "./spatial_ct_ct_interactions/L2_multi_linear/TopCoeff_R0/*.png"
+        coeff_cutoff=20 # No. of coefficient want to show in the x axis of the figure
+
+        figsize_eval=[4,3]  #width and height of the figure in "./spatial_ct_ct_interactions/L2_multi_linear/scores_0.png"
+        figsize_niche=[10,7] #width and height of the figure in "./spatial_ct_ct_interactions/L2_multi_linear/scores_0.png"
+        niche_cutoff=0.12  #cutoff use for plotting the niche interactions map
+        '''
+
+        BothLinearAndCrossTerms=1# If only linear terms then put 1; For both linear and crossterms use 2
+        strategy='L2_multi' #Name of the strategy you want to compute the interactions options are [L1_multi, L1_ovr, L2_multi, L2_ovr, elasticnet_multi, elasticnet_ovr]
+        #strategy='L1_ovr'
+        #strategy='elasticnet_multi'
+
+
+        create_directory(outputdir)
+
+
+        PP,cluster,noct,fraction_CT,clusterWithBarcodeId= reading_data(pos_file,cluster_file,CTname_file,outputdir,delimiter,removed_CTs_before_finding_CT_CT_interactions)
+        M, neighbors,distance=create_spatial_CT_feature_matrix(Radius,PP,cluster,noct,fraction_CT,outputdir)
+        pickle.dump(neighbors,open(outputdir+'save_neighbors_'+str(Radius)+'.p', 'wb'))
+        pickle.dump(distance,open(outputdir+'save_distances_'+str(Radius)+'.p','wb'))
+        df=pd.DataFrame(clusterWithBarcodeId)
+        df.to_csv(outputdir+'save_clusterid_'+str(Radius)+'.csv',index=False)
+
+
+
+
+        f=open(outputdir+'BiologicalNameOfCT.dat')
         nameOfCellType={}
         for line in f:
             l=line[0:-1].split('\t')
             nameOfCellType[int(l[0])]=l[1]
 
         if BothLinearAndCrossTerms==1:
-            maindir=inputdir+strategy+'_linear/'
+            maindir=outputdir+strategy+'_linear/'
         else:
-            maindir=inputdir+strategy+'_cross/'
+            maindir=outputdir+strategy+'_cross/'
 
         create_directory(maindir)
         confusion_cutoff=0 # no of cell types wants to print
 
-        fw=open(maindir+'prediction_R'+str(radius)+'.dat','w')
-        fw.write('\nRadius = '+ str(radius)  + '\n')
-        fname=maindir+'save_numpy_array_'+str(radius)+'.npz'
+        fw=open(maindir+'prediction_R'+str(Radius)+'.dat','w')
+        fw.write('\nRadius = '+ str(Radius)  + '\n')
+        fname=maindir+'save_numpy_array_'+str(Radius)+'.npz'
 
 
         flag=1
         if os.path.isfile(fname):
             filesize = os.path.getsize(fname)
             if filesize>0:
                 data=np.load(fname,allow_pickle=True)
                 coef=data['coef']
                 cmn=data['cmn']
                 cmn_std=data['cmn_std']
                 coef_std=data['coef_std']
                 CTFeatures=data['CTFeatures']
-                find_interacting_cell_types(cmn,coef,cmn_std,coef_std,confusion_cutoff,coeff_cutoff,CTFeatures,nameOfCellType,fw,maindir+'/TopCoeff_R'+str(radius),figuresize)
+                find_interacting_cell_types(cmn,coef,cmn_std,coef_std,confusion_cutoff,coeff_cutoff,CTFeatures,nameOfCellType,fw,maindir+'/TopCoeff_R'+str(Radius),figsize)
                 flag=0
 
 
         if flag==1:
 
                 start_time = time.time()
-                neighborhoodClass,target,inputFeatures=read_processed_data(radius,inputdir)
+                neighborhoodClass,target,inputFeatures=read_processed_data(Radius,outputdir)
                 cmn,coef,comp_score,cmn_std,coef_std,comp_score_std,classes,lambda_c,CTFeatures,x_test,x_train,predicted_probs,fpr, tpr, roc_auc=model_log_regression(K_fold, n_repeats,neighborhoodClass,target,lambda_c_ranges,strategy,BothLinearAndCrossTerms,seed,n_jobs)
-                np.savetxt(maindir+'matrix_avg_coefficients_R'+str(radius)+'.dat', coef,fmt='%0.6f',delimiter=',')
-                np.savetxt(maindir+'matrix_avg_confusion_R'+str(radius)+'.dat', cmn,fmt='%0.6f',delimiter=',')
+                np.savetxt(maindir+'matrix_avg_coefficients_R'+str(Radius)+'.dat', coef,fmt='%0.6f',delimiter=',')
+                np.savetxt(maindir+'matrix_avg_confusion_R'+str(Radius)+'.dat', cmn,fmt='%0.6f',delimiter=',')
                 score=np.array([comp_score, comp_score_std]).T
-                np.savetxt(maindir+'matrix_std_coefficients_R'+str(radius)+'.dat', coef_std,fmt='%0.6f',delimiter=',')
-                np.savetxt(maindir+'matrix_std_confusion_R'+str(radius)+'.dat', cmn_std,fmt='%0.6f',delimiter=',')
-                np.savetxt(maindir+'matrix_score_R'+str(radius)+'.dat',score ,fmt='%0.4f',delimiter=',')
+                np.savetxt(maindir+'matrix_std_coefficients_R'+str(Radius)+'.dat', coef_std,fmt='%0.6f',delimiter=',')
+                np.savetxt(maindir+'matrix_std_confusion_R'+str(Radius)+'.dat', cmn_std,fmt='%0.6f',delimiter=',')
+                np.savetxt(maindir+'matrix_score_R'+str(Radius)+'.dat',score ,fmt='%0.4f',delimiter=',')
                 #np.savetxt(maindir+'matrix_Features'+str(radius)+'.dat',CTFeatures ,fmt='%s',delimiter=',')
-                np.savez(maindir+'save_numpy_array_'+str(radius)+'.npz',cmn=cmn,coef=coef,cmn_std=cmn_std,coef_std=coef_std,CTFeatures=CTFeatures)
+                np.savez(maindir+'save_numpy_array_'+str(Radius)+'.npz',cmn=cmn,coef=coef,cmn_std=cmn_std,coef_std=coef_std,CTFeatures=CTFeatures)
 
-                find_interacting_cell_types(cmn,coef,cmn_std,coef_std,confusion_cutoff,coeff_cutoff,CTFeatures,nameOfCellType,fw,maindir+'/TopCoeff_R'+str(radius),figuresize)
+                find_interacting_cell_types(cmn,coef,cmn_std,coef_std,confusion_cutoff,coeff_cutoff,CTFeatures,nameOfCellType,fw,maindir+'/TopCoeff_R'+str(Radius),figsize)
 
 
-                plot_results(maindir,2,3,nameOfCellType,radius,lambda_c,cmn,coef,classes,CTFeatures,x_test,x_train,predicted_probs,inputFeatures,BothLinearAndCrossTerms,inputdir,fpr, tpr, roc_auc)
+                plot_results(maindir,2,3,nameOfCellType,Radius,lambda_c,cmn,coef,classes,CTFeatures,x_test,x_train,predicted_probs,inputFeatures,BothLinearAndCrossTerms,outputdir,fpr, tpr, roc_auc)
                 finish_time=time.time()
 
                 fw.write('\n\nTotal time to compute = '+ str(finish_time-start_time)+'\n')
                 print('time taken in sec', finish_time-start_time)
 
         fw.close()
 
+        plot_evaluation_scores(outputdir,Radius,figsize_eval)
+        plot_niche_interactions(outputdir,Radius,figsize_niche,niche_cutoff)
 
 
-def plot_evaluation_scores(inputRadius,BothLinearAndCrossTerms,inputdir,strategy,figuresize):
+
+
+
+def plot_evaluation_scores(outputdir,Radius,figsize):
+
+    BothLinearAndCrossTerms=1
+    strategy='L2_multi'
     if BothLinearAndCrossTerms==1:
-        maindir=inputdir+strategy+'_linear/'
+        maindir=outputdir+strategy+'_linear/'
     else:
-        maindir=inputdir+strategy+'_cross/'
+        maindir=outputdir+strategy+'_cross/'
 
     ## The order of all 15 scores are following
     #1-4 'accuracy','macro F1','macro precision','macro recall',
     #5-7 'micro [all]',
     #8-11 'weighted F1','weighted precision','weighted recall','cohen kappa',
     #12=15 'cross entropy', 'matthew correlation coefficient','heming loss', 'zero one loss'
 
     xlabels=['accuracy','macro F1','macro precision','macro recall','micro [all]','weighted F1','weighted precision','weighted recall','cohen kappa','mcc']
     index=[0,1,2,3,4,7,8,9,10,12]
 
-    for radius in inputRadius:
-        fig,axs=plt.subplots(1,1,figsize=(figuresize[0],figuresize[1]))
-        name=maindir+'matrix_score_R'+str(radius)+'.dat'
-        data=np.genfromtxt(open(name, "rb"), delimiter=',', skip_header=0)
-        yt=data[index,0]
-        xt=range(len(yt))
-        axs.plot(xt,yt,'b.-',label=strategy)
-        lowRg=yt-data[index,1]
-        highRg=yt+data[index,1]
-        axs.fill_between(xt, lowRg, highRg,facecolor='b',alpha=0.2)
-        legend1= axs.legend(loc='lower left',bbox_to_anchor=(0.02, 0.05),ncol=1, borderaxespad=0., prop={"size":6},fancybox=True, shadow=True)
-
-        axs.set_xticks(range(len(index)))
-        ytstd=max(data[index,1])
-        axs.set_yticks(np.linspace(min(yt)-ytstd,max(yt)+ytstd,4))
-
-        axs.set_xticklabels(xlabels)
-        for tick in axs.get_xticklabels():
-            tick.set_rotation(90)
-
-        axs.set_ylabel('score')
-        fig.tight_layout()
-        fig.savefig(maindir+'scores_'+str(radius)+'.png',bbox_inches='tight',dpi=300)
-        fig.clf()
+    fig,axs=plt.subplots(1,1,figsize=(figsize[0],figsize[1]))
+    name=maindir+'matrix_score_R'+str(Radius)+'.dat'
+    data=np.genfromtxt(open(name, "rb"), delimiter=',', skip_header=0)
+    yt=data[index,0]
+    xt=range(len(yt))
+    axs.plot(xt,yt,'b.-',label=strategy)
+    lowRg=yt-data[index,1]
+    highRg=yt+data[index,1]
+    axs.fill_between(xt, lowRg, highRg,facecolor='b',alpha=0.2)
+    legend1= axs.legend(loc='lower left',bbox_to_anchor=(0.02, 0.05),ncol=1, borderaxespad=0., prop={"size":6},fancybox=True, shadow=True)
+
+    axs.set_xticks(range(len(index)))
+    ytstd=max(data[index,1])
+    axs.set_yticks(np.linspace(min(yt)-ytstd,max(yt)+ytstd,4))
+
+    axs.set_xticklabels(xlabels)
+    for tick in axs.get_xticklabels():
+        tick.set_rotation(90)
+
+    axs.set_ylabel('score')
+    fig.tight_layout()
+    fig.savefig(maindir+'scores_'+str(Radius)+'.png',bbox_inches='tight',dpi=300)
+    fig.clf()
 
 
 
 def plot_normalized_coefficients_radius_wise(inputRadius,BothLinearAndCrossTerms,inputdir,strategy,figuresize):
     f=open(inputdir+'BiologicalNameOfCT.dat')
     nameOfCellType={}
     featureName=[]
@@ -945,34 +1011,36 @@
         fig.tight_layout()
         fig.savefig(savedir+'CT_'+str(i+1)+ '_'+featureName[i]  + '.png',bbox_inches='tight',dpi=300)
         fig.clf()
 
 
 
 
-def plot_niche_interactions(inputdir,strategy,BothLinearAndCrossTerms,radius,figuresize,niche_cutoff):
-#def plot_niche_interactions(inputdir,n_repeats,K_fold,coeff_cutoff,strategy,seed,n_jobs,lambda_c_ranges,BothLinearAndCrossTerms,radius,figuresize):
-        f=open(inputdir+'BiologicalNameOfCT.dat')
+def plot_niche_interactions(outputdir='./spatial_ct_ct_interactions/',Radius=0,figsize_niche=[10,7],niche_cutoff=0.1):
+        #niche_cutoff it is normalized large value has fewer connections and small value has larger connections
+        BothLinearAndCrossTerms=1
+        strategy='L2_multi'
+        f=open(outputdir+'BiologicalNameOfCT.dat')
         nameOfCellType=[]
         for line in f:
             l=line[0:-1].split('\t')
             #nameOfCellType[int(l[0])]=l[1]
             nameOfCellType.append(l[1])
 
         if BothLinearAndCrossTerms==1:
-            maindir=inputdir+strategy+'_linear/'
+            maindir=outputdir+strategy+'_linear/'
         else:
-            maindir=inputdir+strategy+'_cross/'
+            maindir=outputdir+strategy+'_cross/'
 
         #create_directory(maindir)
         #confusion_cutoff=0 # no of cell types wants to print
 
         #fw=open(maindir+'prediction_R'+str(radius)+'.dat','w')
         #fw.write('\nRadius = '+ str(radius)  + '\n')
-        fname=maindir+'save_numpy_array_'+str(radius)+'.npz'
+        fname=maindir+'save_numpy_array_'+str(Radius)+'.npz'
         #print('fname',fname)
         flag=1
         if os.path.isfile(fname):
             filesize = os.path.getsize(fname)
             if filesize>0:
                 data=np.load(fname,allow_pickle=True)
                 coef=data['coef']
@@ -1005,27 +1073,27 @@
         coeff_of_CT.append(meanCoefficients[i])
         name_of_the_coeff.append(temp)
         std_of_coeff.append(stdCoefficients[i])
         '''
         #sklearn.cluster.bicluster
         linked=linkage(coef,'single')
         #plt.figure(figsize=(10, 7))
-        fig,ax=plt.subplots( figsize=(figuresize[0],figuresize[1]))
+        fig,ax=plt.subplots( figsize=(figsize_niche[0],figsize_niche[1]))
         dendrogram(linked,
             orientation='top',
             labels=nameOfCellType,
             distance_sort='descending',
             show_leaf_counts=True)
         #ax.set_xticks(xx)
         #ax.set_xticklabels(name_of_the_coeff)
         for tick in ax.get_xticklabels():
             tick.set_rotation(90)
 
-        fig.savefig(maindir+'HierarchicalClustering_Rad'+str(radius),bbox_inches='tight',dpi=300)
-        fig.clf()
+        fig.savefig(maindir+'HierarchicalClustering_Rad'+str(Radius),bbox_inches='tight',dpi=300)
+        plt.close('all')
 
 
 
 
 
 
         n=len(nameOfCellType)
@@ -1037,15 +1105,15 @@
         #coef=coef[0:3,0:19]
 
         labeldict={}
         for i in range(len(nameOfCellType)):
             labeldict[i]=nameOfCellType[i]
             G.add_node(i,color=gradientColor[i])
 
-        fig,ax=plt.subplots( figsize=(figuresize[0],figuresize[1]))
+        fig,ax=plt.subplots( figsize=(figsize_niche[0],figsize_niche[1]))
         edges=[]
         #print('coef',coef.shape, np.max(abs(coef)))
         norm_coef=coef/np.max(abs(coef))
 
         largest=[]
         for i in range(coef.shape[0]):
             for j in range(coef.shape[1]):
@@ -1089,9 +1157,8 @@
          linewidths=1, font_size=5, font_weight='bold',width=weights, edge_color=colors,node_color=gradientColor,
         )
         nx.draw_networkx_edge_labels(G, pos,edge_labels=edge_labels,label_pos=0.35, font_size=3  )
 
         #plt.show()
 
 
-        fig.savefig(maindir+'DirectedGraph_Rad'+str(radius),bbox_inches='tight',dpi=300)
-        fig.clf()
+        fig.savefig(maindir+'DirectedGraph_Rad'+str(Radius),bbox_inches='tight',dpi=300)
```

### Comparing `nico_sc_sp-0.0.2/nico/__init__.py` & `nico-sc-sp-0.0.3/nico/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from nico.Spatial_Annotations import find_index
 from nico.Spatial_Annotations import find_match_index_in_dist
 from nico.Spatial_Annotations import find_mutual_nn
 from nico.Spatial_Annotations import sct_return_sc_sp_in_shared_common_PC_space
 from nico.Spatial_Annotations import degree_based_annotation
 from nico.Spatial_Annotations import find_annotation_index
 from nico.Spatial_Annotations import find_commnon_MNN
-from nico.Spatial_Annotations import built_MNN_matrix_between_sc_and_sp
+from nico.Spatial_Annotations import find_anchor_cells_between_ref_and_query
 from nico.Spatial_Annotations import read_KNN_file
 from nico.Spatial_Annotations import return_singlecells
 from nico.Spatial_Annotations import findSpatialCells
 from nico.Spatial_Annotations import find_all_the_spatial_cells_mapped_to_single_cells
 from nico.Spatial_Annotations import write_annotation
 from nico.Spatial_Annotations import find_unmapped_cells_and_deg
 from nico.Spatial_Annotations import resolved_confused_and_unmapped_mapping_of_cells_distance
@@ -23,15 +23,15 @@
 from nico.Spatial_Interactions import reading_data
 from nico.Spatial_Interactions import plot_multiclass_roc
 from nico.Spatial_Interactions import plot_results
 from nico.Spatial_Interactions import read_processed_data
 from nico.Spatial_Interactions import calculate_class_weights
 from nico.Spatial_Interactions import model_log_regression
 from nico.Spatial_Interactions import find_interacting_cell_types
-from nico.Spatial_Interactions import run_logistic_regression_on_spatial_features
+from nico.Spatial_Interactions import spatial_neighborhood_analysis
 from nico.Spatial_Interactions import plot_evaluation_scores
 from nico.Spatial_Interactions import plot_normalized_coefficients_radius_wise
 from nico.Spatial_Interactions import plot_niche_interactions
 from nico.Spatial_Covariations import create_directory
 from nico.Spatial_Covariations import find_index
 from nico.Spatial_Covariations import read_spatial_data
 from nico.Spatial_Covariations import find_correlation_bw_genes_and_PC_component_in_singlecell
@@ -43,15 +43,15 @@
 from nico.Spatial_Covariations import makePCneighboorhoodFeatureMatrix
 from nico.Spatial_Covariations import compute_PC_space
 from nico.Spatial_Covariations import model_linear_regression
 from nico.Spatial_Covariations import run_ridge_regression
 from nico.Spatial_Covariations import find_logistic_regression_interacting_score
 from nico.Spatial_Covariations import chooseRightColorBarForPvalue
 from nico.Spatial_Covariations import plot_results
-from nico.Spatial_Covariations import main
+from nico.Spatial_Covariations import gene_covariation_analysis
 from nico.Spatial_Covariations import pathway_analysis
 from nico.Spatial_Covariations import find_canonical_pathways_in_interacting_cell_types
 from nico.Spatial_Covariations import find_fold_change
 from nico.Spatial_Covariations import made_excel_sheet_for_gene_correlation
 from nico.Spatial_Covariations import triangulation_for_triheatmap
 from nico.Spatial_Covariations import plot_ligand_receptor_in_interacting_celltypes
 from nico.Spatial_Covariations import read_LigRecDb
```

### Comparing `nico_sc_sp-0.0.2/nico/utilities/SCTransform.py` & `nico-sc-sp-0.0.3/nico/utilities/SCTransform.py`

 * *Files identical despite different names*

### Comparing `nico_sc_sp-0.0.2/nico/utilities/__init__.py` & `nico-sc-sp-0.0.3/nico/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `nico_sc_sp-0.0.2/nico/utilities/pyliger_utilities.py` & `nico-sc-sp-0.0.3/nico/utilities/pyliger_utilities.py`

 * *Files identical despite different names*

### Comparing `nico_sc_sp-0.0.2/setup.py` & `nico-sc-sp-0.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Find covariation patterns between interacted cell types from spatial data'
 LONG_DESCRIPTION = 'A package that perform cell type annotations on spatial transcriptomics data, find the niche interactions and covariation patterns between interacted cell types'
 
 # Setting up
-setup(
-    name="nico_sc_sp",
+setup(name="nico-sc-sp",
     version=VERSION,
     author="Ankit Agrawal",
     author_email="<ankitplusplus@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['opencv-python'],
-    keywords=['python', 'niche','spatial transcriptomics','single-cell rna sequencing','scRNAseq','nico'],
+    install_requires=['xlsxwriter', 'gseapy', 'scanpy', 'shap', 'pydot', 'KDEpy', 'seaborn','scipy', 'matplotlib','numpy','xgboost', 'leidenalg'],
+    keywords=['python', 'niche','spatial transcriptomics','single-cell RNA sequencing','scRNAseq','nico'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

