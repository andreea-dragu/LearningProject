<script lang="ts">
  import Modal from "./Modal.svelte"
  export let list = [
    {
      id: 1,
      name: 'Blisse Fitzsymon',
      email: 'bfitzsymon0@last.fm',
      gender: 'Female',
    },
    {
      id: 2,
      name: 'Alonso Hendrix',
      email: 'ahendrix1@smugmug.com',
      gender: 'Genderqueer',
    },
    {
      id: 3,
      name: 'Norrie Megany',
      email: 'nmegany2@imgur.com',
      gender: 'Male',
    },
    {
      id: 4,
      name: 'Emanuele Urwen',
      email: 'eurwen3@chronoengine.com',
      gender: 'Male',
    },
    {
      id: 5,
      name: 'Morly Bradnum',
      email: 'mbradnum4@liveinternet.ru',
      gender: 'Male',
    },
    {
      id: 6,
      name: 'Orrin Hailey',
      email: 'ohailey5@europa.eu',
      gender: 'Polygender',
    },
    {
      id: 7,
      name: 'Ira Kyncl',
      email: 'ikyncl6@amazon.de',
      gender: 'Bigender',
    },
    {
      id: 8,
      name: 'Hilary Micheu',
      email: 'hmicheu7@networkadvertising.org',
      gender: 'Non-binary',
    },
    {
      id: 9,
      name: 'Antin Nesey',
      email: 'anesey8@sitemeter.com',
      gender: 'Male',
    },
    {
      id: 10,
      name: 'Olivero Cariss',
      email: 'ocariss9@w3.org',
      gender: 'Male',
    },
    {
      id: 11,
      name: 'Gerry Dallimare',
      email: 'gdallimarea@sphinn.com',
      gender: 'Male',
    },
    {
      id: 12,
      name: 'Ariela Capun',
      email: 'acapunb@hibu.com',
      gender: 'Female',
    },
    {
      id: 13,
      name: 'Dru Heilds',
      email: 'dheildsc@howstuffworks.com',
      gender: 'Male',
    },
    {
      id: 14,
      name: 'Bond Kivelle',
      email: 'bkivelled@163.com',
      gender: 'Male',
    },
    {
      id: 15,
      name: 'Rodolfo Langton',
      email: 'rlangtone@tiny.cc',
      gender: 'Male',
    },
    {
      id: 16,
      name: 'Barri Garrad',
      email: 'bgarradf@google.ca',
      gender: 'Male',
    },
    {
      id: 17,
      name: 'Janeen Boxell',
      email: 'jboxellg@yale.edu',
      gender: 'Female',
    },
    {
      id: 18,
      name: 'Caye Bordman',
      email: 'cbordmanh@dell.com',
      gender: 'Female',
    },
    {
      id: 19,
      name: 'Daron Duchateau',
      email: 'dduchateaui@elpais.com',
      gender: 'Male',
    },
    {
      id: 20,
      name: 'Gonzales Feldbau',
      email: 'gfeldbauj@psu.edu',
      gender: 'Male',
    },
    {
      id: 21,
      name: 'Hayden Borless',
      email: 'hborlessk@elpais.com',
      gender: 'Male',
    },
    {
      id: 22,
      name: 'Jakob Piatti',
      email: 'jpiattil@e-recht24.de',
      gender: 'Male',
    },
    {
      id: 23,
      name: 'Philis Leatherbarrow',
      email: 'pleatherbarrowm@amazon.com',
      gender: 'Female',
    },
    {
      id: 24,
      name: 'Joe Beric',
      email: 'jbericn@quantcast.com',
      gender: 'Male',
    },
    {
      id: 25,
      name: 'Sauncho Duckering',
      email: 'sduckeringo@foxnews.com',
      gender: 'Male',
    },
    {
      id: 26,
      name: 'Feodor Straffon',
      email: 'fstraffonp@linkedin.com',
      gender: 'Male',
    },
    {
      id: 27,
      name: 'Leda Nottingham',
      email: 'lnottinghamq@mtv.com',
      gender: 'Female',
    },
    {
      id: 28,
      name: 'Ignatius Kase',
      email: 'ikaser@ebay.com',
      gender: 'Male',
    },
    {
      id: 29,
      name: 'Kaja Vinter',
      email: 'kvinters@qq.com',
      gender: 'Female',
    },
    {
      id: 30,
      name: 'Cynthia Quarterman',
      email: 'cquartermant@umich.edu',
      gender: 'Female',
    },
    {
      id: 31,
      name: 'Hewet Zmitruk',
      email: 'hzmitruku@mayoclinic.com',
      gender: 'Male',
    },
    {
      id: 32,
      name: 'Giorgio Garrat',
      email: 'ggarratv@posterous.com',
      gender: 'Male',
    },
    {
      id: 33,
      name: 'Franky Easeman',
      email: 'feasemanw@homestead.com',
      gender: 'Male',
    },
    {
      id: 34,
      name: 'Claire Poluzzi',
      email: 'cpoluzzix@cnet.com',
      gender: 'Female',
    },
    {
      id: 35,
      name: 'Nonna Germon',
      email: 'ngermony@samsung.com',
      gender: 'Female',
    },
    {
      id: 36,
      name: 'Allissa Poile',
      email: 'apoilez@craigslist.org',
      gender: 'Female',
    },
    {
      id: 37,
      name: 'Sheela Domerque',
      email: 'sdomerque10@amazon.com',
      gender: 'Female',
    },
    {
      id: 38,
      name: 'Ofilia Brace',
      email: 'obrace11@facebook.com',
      gender: 'Female',
    },
    {
      id: 39,
      name: 'Shawnee Meggison',
      email: 'smeggison12@ask.com',
      gender: 'Female',
    },
    {
      id: 40,
      name: 'Gracia Trebble',
      email: 'gtrebble13@japanpost.jp',
      gender: 'Female',
    },
    {
      id: 41,
      name: 'Pattie Moir',
      email: 'pmoir14@fastcompany.com',
      gender: 'Female',
    },
    {
      id: 42,
      name: 'Sophie Ivanyutin',
      email: 'sivanyutin15@etsy.com',
      gender: 'Agender',
    },
    {
      id: 43,
      name: 'Cad Lujan',
      email: 'clujan16@un.org',
      gender: 'Male',
    },
    {
      id: 44,
      name: 'Elianore Confait',
      email: 'econfait17@desdev.cn',
      gender: 'Female',
    },
    {
      id: 45,
      name: 'Darla Matthessen',
      email: 'dmatthessen18@unc.edu',
      gender: 'Female',
    },
    {
      id: 46,
      name: 'Titos Coon',
      email: 'tcoon19@linkedin.com',
      gender: 'Male',
    },
    {
      id: 47,
      name: 'Katharyn Reddie',
      email: 'kreddie1a@statcounter.com',
      gender: 'Bigender',
    },
    {
      id: 48,
      name: 'Farlee Carwithim',
      email: 'fcarwithim1b@taobao.com',
      gender: 'Male',
    },
    {
      id: 49,
      name: 'Piotr Depka',
      email: 'pdepka1c@google.es',
      gender: 'Male',
    },
    {
      id: 50,
      name: 'Farrand Benezet',
      email: 'fbenezet1d@lulu.com',
      gender: 'Polygender',
    },
    {
      id: 51,
      name: 'Aurelea Luney',
      email: 'aluney1e@gnu.org',
      gender: 'Female',
    },
    {
      id: 52,
      name: 'Gardner Benn',
      email: 'gbenn1f@mozilla.org',
      gender: 'Male',
    },
    {
      id: 53,
      name: 'Amelina Rowthorne',
      email: 'arowthorne1g@freewebs.com',
      gender: 'Female',
    },
    {
      id: 54,
      name: 'Tanhya Cumberland',
      email: 'tcumberland1h@booking.com',
      gender: 'Female',
    },
    {
      id: 55,
      name: 'Brice Fishwick',
      email: 'bfishwick1i@timesonline.co.uk',
      gender: 'Male',
    },
    {
      id: 56,
      name: 'Paxon Ivanshintsev',
      email: 'pivanshintsev1j@si.edu',
      gender: 'Male',
    },
    {
      id: 57,
      name: 'Quent Wright',
      email: 'qwright1k@aol.com',
      gender: 'Male',
    },
    {
      id: 58,
      name: "Jarrad O'Currigan",
      email: 'jocurrigan1l@yellowbook.com',
      gender: 'Male',
    },
    {
      id: 59,
      name: 'Carson Apted',
      email: 'capted1m@yellowbook.com',
      gender: 'Polygender',
    },
    {
      id: 60,
      name: 'Ritchie Buttner',
      email: 'rbuttner1n@accuweather.com',
      gender: 'Male',
    },
    {
      id: 61,
      name: 'Priscilla Dutton',
      email: 'pdutton1o@theglobeandmail.com',
      gender: 'Female',
    },
    {
      id: 62,
      name: 'Emmett Rhymes',
      email: 'erhymes1p@forbes.com',
      gender: 'Male',
    },
    {
      id: 63,
      name: 'Fae Trethowan',
      email: 'ftrethowan1q@jugem.jp',
      gender: 'Female',
    },
    {
      id: 64,
      name: 'Nobe Ocheltree',
      email: 'nocheltree1r@e-recht24.de',
      gender: 'Male',
    },
    {
      id: 65,
      name: 'Stephi Reasun',
      email: 'sreasun1s@shop-pro.jp',
      gender: 'Female',
    },
    {
      id: 66,
      name: 'Lian Seckom',
      email: 'lseckom1t@exblog.jp',
      gender: 'Female',
    },
    {
      id: 67,
      name: 'Elyssa Fibbitts',
      email: 'efibbitts1u@patch.com',
      gender: 'Female',
    },
    {
      id: 68,
      name: 'Wini Gouda',
      email: 'wgouda1v@census.gov',
      gender: 'Female',
    },
    {
      id: 69,
      name: 'Amalita Championnet',
      email: 'achampionnet1w@tinypic.com',
      gender: 'Female',
    },
    {
      id: 70,
      name: 'Ansell Tredget',
      email: 'atredget1x@360.cn',
      gender: 'Male',
    },
    {
      id: 71,
      name: 'Moselle Kerbey',
      email: 'mkerbey1y@123-reg.co.uk',
      gender: 'Genderqueer',
    },
    {
      id: 72,
      name: 'Daile Wasiel',
      email: 'dwasiel1z@discuz.net',
      gender: 'Female',
    },
    {
      id: 73,
      name: 'Alberta Kaemena',
      email: 'akaemena20@squidoo.com',
      gender: 'Agender',
    },
    {
      id: 74,
      name: 'Irwin Tussaine',
      email: 'itussaine21@unc.edu',
      gender: 'Male',
    },
    {
      id: 75,
      name: 'Chaddy Heynen',
      email: 'cheynen22@usnews.com',
      gender: 'Male',
    },
    {
      id: 76,
      name: 'Jereme McAndrew',
      email: 'jmcandrew23@fema.gov',
      gender: 'Male',
    },
    {
      id: 77,
      name: 'Tan Callum',
      email: 'tcallum24@amazon.de',
      gender: 'Male',
    },
    {
      id: 78,
      name: 'Mindy Liptrot',
      email: 'mliptrot25@noaa.gov',
      gender: 'Female',
    },
    {
      id: 79,
      name: 'Margareta McMackin',
      email: 'mmcmackin26@unesco.org',
      gender: 'Female',
    },
    {
      id: 80,
      name: 'Farly Tiron',
      email: 'ftiron27@wiley.com',
      gender: 'Male',
    },
    {
      id: 81,
      name: 'Glynis Amy',
      email: 'gamy28@chron.com',
      gender: 'Female',
    },
    {
      id: 82,
      name: 'Susann Breton',
      email: 'sbreton29@ucsd.edu',
      gender: 'Female',
    },
    {
      id: 83,
      name: 'Miguela Howcroft',
      email: 'mhowcroft2a@github.com',
      gender: 'Female',
    },
    {
      id: 84,
      name: 'Feodor Kivell',
      email: 'fkivell2b@vinaora.com',
      gender: 'Male',
    },
    {
      id: 85,
      name: 'Odele Burgill',
      email: 'oburgill2c@eventbrite.com',
      gender: 'Female',
    },
    {
      id: 86,
      name: 'Bard Feldstern',
      email: 'bfeldstern2d@unicef.org',
      gender: 'Male',
    },
    {
      id: 87,
      name: 'Codee MacShirrie',
      email: 'cmacshirrie2e@kickstarter.com',
      gender: 'Female',
    },
    {
      id: 88,
      name: 'Charley Eymor',
      email: 'ceymor2f@amazon.co.jp',
      gender: 'Male',
    },
    {
      id: 89,
      name: 'Antonin Jacqueminet',
      email: 'ajacqueminet2g@mediafire.com',
      gender: 'Male',
    },
    {
      id: 90,
      name: 'Arturo Minichi',
      email: 'aminichi2h@psu.edu',
      gender: 'Male',
    },
    {
      id: 91,
      name: 'Tyrus Ponter',
      email: 'tponter2i@java.com',
      gender: 'Male',
    },
    {
      id: 92,
      name: 'Vernon Lowndesbrough',
      email: 'vlowndesbrough2j@yolasite.com',
      gender: 'Male',
    },
    {
      id: 93,
      name: 'Rancell Pahlsson',
      email: 'rpahlsson2k@bing.com',
      gender: 'Male',
    },
    {
      id: 94,
      name: 'Dana Caesar',
      email: 'dcaesar2l@google.com',
      gender: 'Female',
    },
    {
      id: 95,
      name: 'Austin Weeke',
      email: 'aweeke2m@nationalgeographic.com',
      gender: 'Male',
    },
    {
      id: 96,
      name: 'Papagena Palffrey',
      email: 'ppalffrey2n@craigslist.org',
      gender: 'Female',
    },
    {
      id: 97,
      name: 'Celka Eliez',
      email: 'celiez2o@vimeo.com',
      gender: 'Female',
    },
    {
      id: 98,
      name: 'Maurita Kelwick',
      email: 'mkelwick2p@state.tx.us',
      gender: 'Female',
    },
    {
      id: 99,
      name: 'Aime Hyne',
      email: 'ahyne2q@cdc.gov',
      gender: 'Female',
    },
    {
      id: 100,
      name: 'Ole Hartil',
      email: 'ohartil2r@creativecommons.org',
      gender: 'Male',
    },
  ]


  function addUser() {

  }

  function editUser(id:number) {

  }

  function deleteUser(id:number) {
    list = list.filter(item => item.id !== id)
  }
</script>

<table>
  <tr>
    <th>NAME</th>
    <th>EMAIL</th>
    <th>GENDER</th>
    <th>ACTIONS</th>
  </tr>
  {#each list as item}
    <tr>
      <td>{item.name}</td>
      <td>{item.email}</td>
      <td>{item.gender}</td>
      <td>
        <button title="Add" on:click={addUser}><svg xmlns="http://www.w3.org/2000/svg" clip-rule="evenodd" fill-rule="evenodd" stroke-linejoin="round" stroke-miterlimit="2" width="24" height="24" viewBox="0 0 24 24"><path d="m12.002 2c5.518 0 9.998 4.48 9.998 9.998 0 5.517-4.48 9.997-9.998 9.997-5.517 0-9.997-4.48-9.997-9.997 0-5.518 4.48-9.998 9.997-9.998zm-.747 9.25h-3.5c-.414 0-.75.336-.75.75s.336.75.75.75h3.5v3.5c0 .414.336.75.75.75s.75-.336.75-.75v-3.5h3.5c.414 0 .75-.336.75-.75s-.336-.75-.75-.75h-3.5v-3.5c0-.414-.336-.75-.75-.75s-.75.336-.75.75z" fill-rule="nonzero"/></svg></button>
        <button title="Edit" on:click={() => editUser(item.id)}><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M5 21h-5v-2h5v2zm3.424-5.718l4.402 4.399-5.826 1.319 1.424-5.718zm15.576-6.748l-9.689 9.804-4.536-4.536 9.689-9.802 4.536 4.534z"/></svg></button>
        <button title="Delete" on:click={() => deleteUser(item.id)}><svg xmlns="http://www.w3.org/2000/svg" clip-rule="evenodd" fill-rule="evenodd" stroke-linejoin="round" stroke-miterlimit="2" width="24" height="24" viewBox="0 0 24 24" ><path d="m12.002 2.005c5.518 0 9.998 4.48 9.998 9.997 0 5.518-4.48 9.998-9.998 9.998-5.517 0-9.997-4.48-9.997-9.998 0-5.517 4.48-9.997 9.997-9.997zm0 8.933-2.721-2.722c-.146-.146-.339-.219-.531-.219-.404 0-.75.324-.75.749 0 .193.073.384.219.531l2.722 2.722-2.728 2.728c-.147.147-.22.34-.22.531 0 .427.35.75.751.75.192 0 .384-.073.53-.219l2.728-2.728 2.729 2.728c.146.146.338.219.53.219.401 0 .75-.323.75-.75 0-.191-.073-.384-.22-.531l-2.727-2.728 2.717-2.717c.146-.147.219-.338.219-.531 0-.425-.346-.75-.75-.75-.192 0-.385.073-.531.22z" fill-rule="nonzero"/></svg></button>
      </td>
    </tr>
  {/each}
</table>

<Modal />