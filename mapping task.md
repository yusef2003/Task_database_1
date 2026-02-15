1st diagram :



musician(*MusicianID*, Name, Address, City, State, Phone)



instrument(*InstrumentID*, Name, Key)



album(*AlbumID*, Title, Author)



song(*SongID*, Title, Date)



musician\_instrument(\*\*\****MusicianID, InstrumentID***\*\*\*)



musician\_album(\*\*\****MusicianID, AlbumID***\*\*\*)



song\_album(\*\*\****SongID, AlbumID***\*\*\*)



musician\_song(\*\*\****MusicianID, SongID***\*\*\*)















2nd diagram:



owner(*OwnerID*, Name)



property(*PropertyID*, Name, Location, ***OwnerID***)



employee(*EmpID*, Name, ***OfficeID***)



sales\_office(*OfficeID*, Num, City, State, Zip)



property\_office(\*\*\****PropertyID, OfficeID***\*\*\*)



property\_manager(\*\*\****PropertyID, EmpID***\*\*\*)



owner\_property(\*\*\****OwnerID, PropertyID***\*\*\*, Percent)













3rd diagram:





ward(*WardID*, Name)



patient(*PatientID*, Name, DOB, ***WardID***)



nurse(*NurseID*, Name, Address, ***WardID***)



consultant(*ConsultantID*, Name)



drug(*DrugCode*, RecDosage)



drug\_brand(\*\*\****DrugCode, BrandName***\*\*\*)



consultant\_patient(\*\*\****ConsultantID, PatientID***\*\*\*)



nurse\_gives(

&nbsp;   \*\****\*NurseID, DrugCode, PatientID, Date, Time***\*\*\*,

&nbsp;   Dosage

)



