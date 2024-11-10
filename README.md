# WGS84 - UTM10N Converter
This is an ongoing project aimed at easing data QA for geographic processes. Currently the application will take a .csv file of features with Longitude and Latitude data, and produce a new file of the same data with Easting and Northing data appended for UTM 10N. This is meant for importing GPS point data into QGIS, but any application where UTM coordinates are needed will work. 
- Longitude and Latitude need to be fields in the .csv, and they must have the first letter capitalized.
- Output data will be a new file, raw data will not be affected.
- Longitude and Latitude must be in Decimal Degrees, please convert any DMS coordinates.
- _I have plans to make a DMS/DD converter to integrate into this application, but that is for a later release._
- If you have fields in the .csv for Northing and Easting, as long as they are spelled in full with the first letter capitalized the converter will populate those fields. Otherwise, Easting and Northing will be appended to the table.
- The order of Longitude, Latitude, Northing, and Easting do not matter in the .csv. The converter will find the appropriate field location.

This software is open source, and open to modification, and is covered by the [GNU General Public License 3.0](https://www.gnu.org/licenses/gpl-3.0.en.html).
