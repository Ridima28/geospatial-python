# Workflow Summary

```
Earth Search STAC API
        │
        ▼
Connect to API
        │
        ▼
Retrieve Available Collections
        │
        ▼
Select Sentinel-2 Collection
        │
        ▼
Create Geographic Point
        │
        ▼
Search Images Covering the Point
        │
        ▼
Display Number of Matching Images
```


Explanation of all the values below-> 

Name: WGS 84 / UTM zone 35N
Axis Info [cartesian]:
- E[east]: Easting (metre)
- N[north]: Northing (metre)
Area of Use:
- name: Between 24°E and 30°E, northern hemisphere between equator and 84°N, onshore and offshore. Belarus. Bulgaria. Central African Republic. Democratic Republic of the Congo (Zaire). Egypt. Estonia. Finland. Greece. Latvia. Lesotho. Libya. Lithuania. Moldova. Norway. Poland. Romania. Russian Federation. Sudan. Svalbard. Türkiye (Turkey). Uganda. Ukraine.
- bounds: (24.0, 0.0, 30.0, 84.0)
Coordinate Operation:
- name: UTM zone 35N
- method: Transverse Mercator
Datum: World Geodetic System 1984 ensemble
- Ellipsoid: WGS 84
- Prime Meridian: Greenwich


## 1. Name of the Projection: UTM Zone 35N
- **UTM (Universal Transverse Mercator)** ek map projection system hai jo Earth ko **60 zones** mein divide karta hai.
- Har zone ki width **6° longitude** hoti hai.
- **Zone 35N** ka matlab hai ki yeh **Northern Hemisphere** ke Zone 35 ke liye use hota hai.

---

## 2. Underlying Datum: WGS84
- **Datum** ek reference system hota hai jo batata hai ki Earth ka shape aur position kaise define ki gayi hai.
- **WGS84 (World Geodetic System 1984)** duniya ka sabse common datum hai.
- GPS (Google Maps, mobile GPS) bhi **WGS84** use karta hai.

**Simple Words:**  
Datum Earth ka reference point hai, jiske basis par coordinates calculate hote hain.

---

## 3. Axis Info
Is CRS (Coordinate Reference System) mein **Cartesian Coordinate System** use hota hai.

Do axes hote hain:

- **Easting (X):** East direction ki distance.
- **Northing (Y):** North direction ki distance.

Dono ki unit **meter (m)** hoti hai.

Yeh latitude-longitude nahi hote, balki **meter-based coordinates** hote hain.

---

## 4. Area of Use
Har UTM zone sirf ek specific area ke liye accurate hota hai.

**UTM Zone 35N** ka use:

- **Longitude:** 24°E se 30°E
- **Latitude:** 0°N se 84°N

Agar is range ke bahar use karoge, to projection ki accuracy kam ho sakti hai.

---

## 5. Coordinate Operation
Earth gol (3D) hai, lekin map flat (2D) hota hai.

Isliye coordinates ko convert karne ke liye ek mathematical method use hota hai.

**UTM Zone 35N** mein yeh method **Transverse Mercator Projection** hai.

Yeh projection un areas ke liye bahut accurate hota hai jinki width sirf kuch degrees longitude hoti hai.

### Conversion Flow

```
Latitude & Longitude
        │
        ▼
Transverse Mercator Projection
        │
        ▼
Easting (X) & Northing (Y) in meters
```

---

## 6. Datum Details
Common datums:

- **WGS84:** GPS aur global mapping ke liye sabse common datum.
- **NAD83 (North American Datum 1983):** North America mein use hota tha.

NAD83 ko future mein naye reference systems se replace kiya ja raha hai taaki aur accurate positioning mil sake.

---

# 📌 Easy Summary

| Term | Meaning (Hinglish) |
|------|---------------------|
| **Projection** | Earth ko flat map par dikhane ka mathematical tareeka. |
| **UTM** | Earth ko 60 zones mein divide karta hai. |
| **Zone 35N** | 24°E–30°E longitude aur Northern Hemisphere ke liye projection. |
| **Datum (WGS84)** | Earth ka reference model jisse coordinates calculate hote hain. |
| **Axis** | Easting (X) aur Northing (Y), dono meter mein. |
| **Coordinate Operation** | Transverse Mercator projection jo latitude-longitude ko meter-based coordinates mein convert karta hai. |
| **Area of Use** | Sirf apne zone ke andar sabse zyada accurate hota hai. |