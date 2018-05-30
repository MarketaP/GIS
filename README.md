# GIS

Here are my notes to Python coding that I always forget

# Reclassify multiple rasters
>>> for i in range(14, 44):
...     out = Reclassify("C:/Users/mpodebradska2/Documents/ArcGIS/Thesis_New/USDM/2007/USDM_2007_" + str(i) +".img", "Value", RemapValue([[0,1],[1,2],[2,3],[3,4],[4,5],["NODATA",0]]),"NODATA")
...     out.save("C:/Users/mpodebradska2/Documents/ArcGIS/Thesis_New/USDM/2007/recl_07_" + str(i) +".img")
