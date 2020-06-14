  
create database odev
create table sinif
{
ogrenci_No int NOT NULL ,
sinifId int FOREIGN KEY REFERENCES sinif(sinifId ),
adi_Soyadi varchar(40),
cinsiyet varchar(5),
ders_Adi varchar(30),
vize int,
final int ,
ortalama as ((vize +final)/2),
PRIMARY KEY(ogrenci_No),
INSERT sinif VALUES (1,4571,'Cem UZAN','Erkek','Matematik',60,70)
}
