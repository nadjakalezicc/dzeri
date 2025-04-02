# gitgit
class Automobil{
constructor(marka, model, godiste, kilometraza, cijena, slika){

    this.marka=marka 
    this.model=model
    this.godiste=godiste
    this.kilometraza=kilometraza
    this.cijena=cijena
    this.slika=slika
    
}
    stampa(){
        console.log(this.marka + " " + this.model + ',')
        
        console.log("prosjek:" + this.kilometraza + ',')
         console.log("godine:" + this.godiste)
    }
    h
    

    filter(manje_od)
    {
        if(this.cijena < manje_od)
        {
            return this
        }
    }

    filter1(manje_od)
    {
        if(this.godiste < manje_od)
        {
            return this
        }
    }
  
}
   automobil = new Automobil( 'BMW', 3, 2000 ,20000, 250, "https://www.bmw-voli.me/content/dam/bmw/common/all-models/3-series/sedan/2024/navigation/bmw-3-series-ice-lci-modelfinder.png")
   automobil1 = new Automobil( 'porshe',911,2000,15, 3000)
    automobil2 = new Automobil( 'bugatti','W16',2010,3, 1000000)
    automobil3 = new Automobil( 'lambo',3, 2020, 17, 500000)
     automobil4 = new Automobil( 'BMW', 4, 2020 ,20000, 30000)
   automobil5 = new Automobil( 'porshe',4,2020,15, 500000)
    automobil6 = new Automobil( 'bugatti','W17',2030,3, 100000)
    automobil7 = new Automobil( 'lambo',7, 2020, 17, 500900)
    automobil8 = new Automobil( 'porshe',10,2010,15, 500000)
    automobil9 = new Automobil( 'bugatti','W47',2010,9567, 2500)
    automobil10 = new Automobil( 'lambo',9, 2020, 156787, 599900)


automobili_niz = [];
automobili_niz.push(automobil1)
automobili_niz.push(automobil2)
automobili_niz.push(automobil3)
automobili_niz.push(automobil4)
automobili_niz.push(automobil5)
automobili_niz.push(automobil6)
automobili_niz.push(automobil7)
automobili_niz.push(automobil8)
automobili_niz.push(automobil9)
automobili_niz.push(automobil10)
novi_niz = [];


for(let i = 0; i<automobili_niz.length; i++)
{
    if(automobili_niz[i].filter(5000))
    {
        if(automobili_niz[i].filter1(2020))
        {
            novi_niz.push(automobili_niz[i])
        }
    }

}

console.log(novi_niz)
