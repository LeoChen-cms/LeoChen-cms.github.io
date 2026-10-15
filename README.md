<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Birdwatching Journal · Fujian</title>
<style>/* ============ 全局基础 ============ */
.bw-page {
  max-width: 960px;
  margin: 0 auto;
  line-height: 1.75;
  color: #2d3a35;
  font-family: -apple-system, "PingFang SC", "Microsoft YaHei", "Segoe UI", sans-serif;
}
.bw-page img { border-radius: 10px; box-shadow: 0 2px 10px rgba(0,0,0,.10); }
.bw-page em { color: #6b7d76; }

/* ============ 顶部简介 ============ */
.bw-hero {
  padding: 28px 32px;
  border-radius: 14px;
  background: linear-gradient(135deg, #eef7f3 0%, #e3f0f7 100%);
  border: 1px solid #d3e4dc;
  margin-bottom: 18px;
}
.bw-hero .bw-tagline { font-size: 1.15em; color: #2f6f5e; font-weight: 600; margin: 0 0 6px; }
.bw-hero .bw-sub { color: #5c6f68; margin: 0; }
.bw-hero .bw-contact { font-size: .9em; color: #7a8a84; margin-top: 10px; }

/* ============ 折叠面板通用 ============ */
.bw-page details {
  border: 1px solid #dde7e2;
  border-radius: 12px;
  margin: 14px 0;
  background: #fbfdfc;
  overflow: hidden;
}
.bw-page summary {
  list-style: none;
  cursor: pointer;
  padding: 14px 18px;
  font-weight: 600;
  font-size: 1.05em;
  color: #24483d;
  background: linear-gradient(90deg, #edf5f1, #f7fbf9);
  border-left: 6px solid #52796f;
  transition: background .15s ease, padding-left .15s ease;
  user-select: none;
}
.bw-page summary::-webkit-details-marker { display: none; }
.bw-page summary::before {
  content: "▸";
  display: inline-block;
  margin-right: 10px;
  color: #52796f;
  transition: transform .18s ease;
  font-size: .95em;
}
.bw-page details[open] summary::before { transform: rotate(90deg); }
.bw-page summary:hover { background: #e2efe8; padding-left: 24px; }
.bw-page details[open] summary { border-bottom: 1px solid #e3ece8; }
.bw-page details > *:not(summary) { margin-left: 18px; margin-right: 18px; }

/* 每个地点板块用不同主题色区分 */
.bw-site summary { border-left-color: var(--accent, #52796f); }
.bw-site summary::before { color: var(--accent, #52796f); }
.bw-site summary:hover { background: color-mix(in srgb, var(--accent, #52796f) 12%, white); }

/* ============ 鸟种名录表格 ============ */
.bw-table-wrap { overflow-x: auto; margin: 12px 0; }
.bw-table-wrap table {
  width: 100%;
  border-collapse: collapse;
  font-size: .95em;
  white-space: nowrap;
}
.bw-table-wrap th {
  background: #52796f;
  color: #fff;
  padding: 8px 12px;
  text-align: left;
  position: sticky;
  top: 0;
}
.bw-table-wrap td { padding: 6px 12px; border-bottom: 1px solid #e6eeea; }
.bw-table-wrap tbody tr:nth-child(even) { background: #f3f8f5; }
.bw-table-wrap tbody tr:hover { background: #e6f1ec; }

/* ============ 物种卡片网格 ============ */
.bw-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
  gap: 20px;
  margin: 20px 0;
}
.bw-card {
  border: 1px solid #e0e9e4;
  border-radius: 12px;
  overflow: hidden;
  background: #fff;
  transition: transform .15s ease, box-shadow .15s ease;
}
.bw-card:hover { transform: translateY(-3px); box-shadow: 0 6px 16px rgba(60,90,80,.15); }
.bw-card img { display: block; width: 100%; height: 190px; object-fit: cover; border-radius: 0; box-shadow: none; }
.bw-card .bw-card-body { padding: 10px 14px 12px; }
.bw-card .bw-card-en { font-weight: 700; color: #24483d; }
.bw-card .bw-card-cn { font-weight: 600; color: #52796f; margin-left: 4px; }
.bw-card .bw-card-sci { font-size: .88em; color: #7a8a84; font-style: italic; }

/* ============ 反思/杂记 ============ */
.bw-notes {
  border-left: 4px solid #c9a86a;
  background: #fdfaf3;
  padding: 14px 18px;
  border-radius: 0 10px 10px 0;
  color: #4d4636;
}

/* ============ ACGN ============ */
.bw-acgn { text-align: center; margin-top: 24px; }
.bw-acgn img { max-width: 420px; width: 100%; }
.bw-acgn p { color: #7a8a84; font-size: .92em; }</style>
<base target="_blank">
</head>
<body>
<div class="bw-page">

<div class="bw-hero">
  <p class="bw-tagline">A personal collection of nature, birdwatching, and everyday observations. 🧭</p>
  <p class="bw-sub"><em>A growing record of the birds and landscapes I have encountered across Fujian, China.</em></p>
  <p class="bw-contact">📮 Contact: 3870045464@qq.com</p>
</div>

<details>
<summary>Bird Species Checklist · 鸟种总名录</summary>

<div class="bw-table-wrap">

<table>
<thead><tr><th>No.</th><th>English Name</th><th>Scientific Name</th><th>中文名</th></tr></thead>
<tbody>
<tr><td>1</td><td>Rufous-capped Babbler</td><td><em>Cyanoderma ruficeps</em></td><td>红头穗鹛</td></tr>
<tr><td>2</td><td>Masked Laughingthrush</td><td><em>Pterorhinus perspicillatus</em></td><td>黑脸噪鹛</td></tr>
<tr><td>3</td><td>Olive-backed Pipit</td><td><em>Anthus hodgsoni</em></td><td>树鹨</td></tr>
<tr><td>4</td><td>Grey Treepie</td><td><em>Dendrocitta formosae</em></td><td>灰树鹊</td></tr>
<tr><td>5</td><td>Great Barbet</td><td><em>Psilopogon virens</em></td><td>大拟啄木鸟</td></tr>
<tr><td>6</td><td>Pallas's Leaf Warbler</td><td><em>Phylloscopus proregulus</em></td><td>黄腰柳莺</td></tr>
<tr><td>7</td><td>Fork-tailed Sunbird</td><td><em>Aethopyga christinae</em></td><td>叉尾太阳鸟</td></tr>
<tr><td>8</td><td>Little Egret</td><td><em>Egretta garzetta</em></td><td>白鹭</td></tr>
<tr><td>9</td><td>Spotted Dove</td><td><em>Spilopelia chinensis</em></td><td>珠颈斑鸠</td></tr>
<tr><td>10</td><td>Chinese Blackbird</td><td><em>Turdus mandarinus</em></td><td>乌鸫</td></tr>
<tr><td>11</td><td>Black-faced Bunting</td><td><em>Emberiza spodocephala</em></td><td>灰头鹀</td></tr>
<tr><td>12</td><td>Oriental Magpie-Robin</td><td><em>Copsychus saularis</em></td><td>鹊鸲</td></tr>
<tr><td>13</td><td>Plumbeous Water Redstart</td><td><em>Phoenicurus fuliginosus</em></td><td>红尾水鸲</td></tr>
<tr><td>14</td><td>White-breasted Waterhen</td><td><em>Amaurornis phoenicurus</em></td><td>白胸苦恶鸟</td></tr>
<tr><td>15</td><td>Little Grebe</td><td><em>Tachybaptus ruficollis</em></td><td>小䴙䴘</td></tr>
<tr><td>16</td><td>Slaty-backed Forktail</td><td><em>Enicurus schistaceus</em></td><td>灰背燕尾</td></tr>
<tr><td>17</td><td>Great Tit</td><td><em>Parus major</em></td><td>大山雀</td></tr>
<tr><td>18</td><td>Black-throated Bushtit</td><td><em>Aegithalos concinnus</em></td><td>红头长尾山雀</td></tr>
<tr><td>19</td><td>White Wagtail</td><td><em>Motacilla alba</em></td><td>白鹡鸰</td></tr>
<tr><td>20</td><td>Grey Wagtail</td><td><em>Motacilla cinerea</em></td><td>灰鹡鸰</td></tr>
<tr><td>21</td><td>Grey-capped Pygmy Woodpecker</td><td><em>Yungipicus canicapillus</em></td><td>星头啄木鸟</td></tr>
<tr><td>22</td><td>Black Bulbul</td><td><em>Hypsipetes leucocephalus</em></td><td>黑短脚鹎</td></tr>
<tr><td>23</td><td>Common Kingfisher</td><td><em>Alcedo atthis</em></td><td>普通翠鸟</td></tr>
<tr><td>24</td><td>Orange-bellied Leafbird</td><td><em>Chloropsis hardwickii</em></td><td>橙腹叶鹎</td></tr>
<tr><td>25</td><td>Light-vented Bulbul</td><td><em>Pycnonotus sinensis</em></td><td>白头鹎</td></tr>
<tr><td>26</td><td>Red-whiskered Bulbul</td><td><em>Pycnonotus jocosus</em></td><td>红耳鹎</td></tr>
<tr><td>27</td><td>Collared Finchbill</td><td><em>Spizixos semitorques</em></td><td>领雀嘴鹎</td></tr>
<tr><td>28</td><td>Mountain Bulbul</td><td><em>Ixos mcclellandii</em></td><td>绿翅短脚鹎</td></tr>
<tr><td>29</td><td>Chestnut Bulbul</td><td><em>Hemixos castanonotus</em></td><td>栗背短脚鹎</td></tr>
<tr><td>30</td><td>Common Sandpiper</td><td><em>Actitis hypoleucos</em></td><td>矶鹬</td></tr>
<tr><td>31</td><td>Red-billed Starling</td><td><em>Spodiopsar sericeus</em></td><td>丝光椋鸟</td></tr>
<tr><td>32</td><td>Richard's Pipit</td><td><em>Anthus richardi</em></td><td>田鹨</td></tr>
<tr><td>33</td><td>Little Ringed Plover</td><td><em>Charadrius dubius</em></td><td>金眶鸻</td></tr>
<tr><td>34</td><td>Dunlin</td><td><em>Calidris alpina</em></td><td>黑腹滨鹬</td></tr>
<tr><td>35</td><td>Plain Prinia</td><td><em>Prinia inornata</em></td><td>纯色山鹪莺</td></tr>
<tr><td>36</td><td>Oriental Magpie</td><td><em>Pica serica</em></td><td>喜鹊</td></tr>
<tr><td>37</td><td>Greater Coucal</td><td><em>Centropus sinensis</em></td><td>褐翅鸦鹃</td></tr>
<tr><td>38</td><td>Yellow Wagtail</td><td><em>Motacilla flava</em></td><td>黄鹡鸰</td></tr>
<tr><td>39</td><td>Grey-capped Greenfinch</td><td><em>Chloris sinica</em></td><td>金翅雀</td></tr>
<tr><td>40</td><td>Little Bunting</td><td><em>Emberiza pusilla</em></td><td>小鹀</td></tr>
<tr><td>41</td><td>Black-winged Kite</td><td><em>Elanus caeruleus</em></td><td>黑翅鸢</td></tr>
<tr><td>42</td><td>Eurasian Tree Sparrow</td><td><em>Passer montanus</em></td><td>麻雀</td></tr>
<tr><td>43</td><td>Cattle Egret</td><td><em>Bubulcus ibis</em></td><td>牛背鹭</td></tr>
<tr><td>44</td><td>Eurasian Spoonbill</td><td><em>Platalea leucorodia</em></td><td>白琵鹭</td></tr>
<tr><td>45</td><td>Spot-billed Duck</td><td><em>Anas zonorhyncha</em></td><td>斑嘴鸭</td></tr>
<tr><td>46</td><td>Eurasian Wigeon</td><td><em>Mareca penelope</em></td><td>赤颈鸭</td></tr>
<tr><td>47</td><td>Eurasian Teal</td><td><em>Anas crecca</em></td><td>绿翅鸭</td></tr>
<tr><td>48</td><td>Long-tailed Shrike</td><td><em>Lanius schach</em></td><td>棕背伯劳</td></tr>
<tr><td>49</td><td>Common Kestrel</td><td><em>Falco tinnunculus</em></td><td>红隼</td></tr>
<tr><td>50</td><td>Grey Heron</td><td><em>Ardea cinerea</em></td><td>苍鹭</td></tr>
<tr><td>51</td><td>Crested Myna</td><td><em>Acridotheres cristatellus</em></td><td>八哥</td></tr>
<tr><td>52</td><td>Grey-backed Shrike</td><td><em>Lanius tephronotus</em></td><td>灰背伯劳</td></tr>
<tr><td>53</td><td>Oriental Turtle Dove</td><td><em>Streptopelia orientalis</em></td><td>山斑鸠</td></tr>
<tr><td>54</td><td>Siberian Crane</td><td><em>Leucogeranus leucogeranus</em></td><td>白鹤</td></tr>
<tr><td>55</td><td>Great Cormorant</td><td><em>Phalacrocorax carbo</em></td><td>普通鸬鹚</td></tr>
<tr><td>56</td><td>Black-headed Gull</td><td><em>Chroicocephalus ridibundus</em></td><td>红嘴鸥</td></tr>
<tr><td>57</td><td>Great Egret</td><td><em>Ardea alba</em></td><td>大白鹭</td></tr>
<tr><td>58</td><td>Peregrine Falcon</td><td><em>Falco peregrinus</em></td><td>游隼</td></tr>
<tr><td>59</td><td>Black Kite</td><td><em>Milvus migrans</em></td><td>黑鸢</td></tr>
<tr><td>60</td><td>Common Greenshank</td><td><em>Tringa nebularia</em></td><td>青脚鹬</td></tr>
<tr><td>61</td><td>Saunders's Gull</td><td><em>Chroicocephalus saundersi</em></td><td>黑嘴鸥</td></tr>
<tr><td>62</td><td>Slaty-backed Gull</td><td><em>Larus schistisagus</em></td><td>西伯利亚银鸥</td></tr>
<tr><td>63</td><td>Common Moorhen</td><td><em>Gallinula chloropus</em></td><td>黑水鸡</td></tr>
<tr><td>64</td><td>Common Snipe</td><td><em>Gallinago gallinago</em></td><td>扇尾沙锥</td></tr>
<tr><td>65</td><td>White-cheeked Starling</td><td><em>Spodiopsar cineraceus</em></td><td>灰椋鸟</td></tr>
<tr><td>66</td><td>Grey Plover</td><td><em>Pluvialis squatarola</em></td><td>灰斑鸻</td></tr>
<tr><td>67</td><td>Black-tailed Godwit</td><td><em>Limosa limosa</em></td><td>黑尾塍鹬</td></tr>
<tr><td>68</td><td>Northern Lapwing</td><td><em>Vanellus vanellus</em></td><td>凤头麦鸡</td></tr>
<tr><td>69</td><td>Black-winged Stilt</td><td><em>Himantopus himantopus</em></td><td>黑翅长脚鹬</td></tr>
<tr><td>70</td><td>Swan Goose</td><td><em>Anser cygnoides</em></td><td>鸿雁</td></tr>
<tr><td>71</td><td>Northern Pintail</td><td><em>Anas acuta</em></td><td>针尾鸭</td></tr>
<tr><td>72</td><td>Taiga Bean Goose</td><td><em>Anser fabalis</em></td><td>豆雁</td></tr>
<tr><td>73</td><td>Tundra Swan</td><td><em>Cygnus columbianus</em></td><td>小天鹅</td></tr>
<tr><td>74</td><td>Mallard</td><td><em>Anas platyrhynchos</em></td><td>绿头鸭</td></tr>
<tr><td>75</td><td>Pied Avocet</td><td><em>Recurvirostra avosetta</em></td><td>反嘴鹬</td></tr>
<tr><td>76</td><td>Bar-tailed Godwit</td><td><em>Limosa lapponica</em></td><td>斑尾塍鹬</td></tr>
<tr><td>77</td><td>Red-billed Leiothrix</td><td><em>Leiothrix lutea</em></td><td>红嘴相思鸟</td></tr>
<tr><td>78</td><td>Japanese White-eye</td><td><em>Zosterops japonicus</em></td><td>暗绿绣眼鸟</td></tr>
<tr><td>79</td><td>Tiger Shrike</td><td><em>Lanius tigrinus</em></td><td>虎纹伯劳</td></tr>
<tr><td>80</td><td>Mugimaki Flycatcher</td><td><em>Ficedula mugimaki</em></td><td>鸲姬鹟</td></tr>
<tr><td>81</td><td>Daurian Redstart</td><td><em>Phoenicurus auroreus</em></td><td>北红尾鸲</td></tr>
<tr><td>82</td><td>Blue Rock-Thrush</td><td><em>Monticola solitarius</em></td><td>蓝矶鸫</td></tr>
<tr><td>83</td><td>Goldcrest</td><td><em>Regulus regulus</em></td><td>戴菊</td></tr>
<tr><td>84</td><td>Eurasian Nuthatch</td><td><em>Sitta europaea</em></td><td>普通䴓</td></tr>
<tr><td>85</td><td>Chestnut-crowned Warbler</td><td><em>Phylloscopus castaniceps</em></td><td>栗头鹟莺</td></tr>
<tr><td>86</td><td>Blue Whistling-Thrush</td><td><em>Myophonus caeruleus</em></td><td>紫啸鸫</td></tr>
<tr><td>87</td><td>Manchurian Bush Warbler</td><td><em>Horornis canturians</em></td><td>远东树莺</td></tr>
</tbody></table>

</div>

</details>

<!-- 01 马尾闽江滨 -->
<details class="bw-site" style="--accent:#4a7ba6" id="mawei">
<summary>01 · 马尾闽江滨 · Mawei Minjiang Riverside <em>— Fuzhou, Fujian · 2026</em></summary>

<div class="bw-grid">

<div class="bw-card"><img src="images/乌鸫_compressed.JPG" alt="乌鸫 Chinese Blackbird"><div class="bw-card-body"><span class="bw-card-en">Chinese Blackbird</span><span class="bw-card-cn">乌鸫</span><div class="bw-card-sci"><em>Turdus mandarinus</em></div></div></div>
<div class="bw-card"><img src="images/柳莺Phylloscopus_compressed.JPG" alt="柳莺 Leaf Warbler"><div class="bw-card-body"><span class="bw-card-en">Leaf Warbler</span><span class="bw-card-cn">柳莺</span><div class="bw-card-sci"><em>Phylloscopus</em></div></div></div>
<div class="bw-card"><img src="images/白胸苦恶鸟_compressed.JPG" alt="白胸苦恶鸟 White-breasted Waterhen"><div class="bw-card-body"><span class="bw-card-en">White-breasted Waterhen</span><span class="bw-card-cn">白胸苦恶鸟</span><div class="bw-card-sci"><em>Amaurornis phoenicurus</em></div></div></div>
<div class="bw-card"><img src="images/白鹭2_compressed.JPG" alt="白鹭 Little Egret"><div class="bw-card-body"><span class="bw-card-en">Little Egret</span><span class="bw-card-cn">白鹭</span><div class="bw-card-sci"><em>Egretta garzetta</em></div></div></div>
<div class="bw-card"><img src="images/青脚鹬_compressed.JPG" alt="青脚鹬 Common Greenshank"><div class="bw-card-body"><span class="bw-card-en">Common Greenshank</span><span class="bw-card-cn">青脚鹬</span><div class="bw-card-sci"><em>Tringa nebularia</em></div></div></div>
<div class="bw-card"><img src="images/黄鹡鸰_compressed.JPG" alt="黄鹡鸰 Yellow Wagtail"><div class="bw-card-body"><span class="bw-card-en">Yellow Wagtail</span><span class="bw-card-cn">黄鹡鸰</span><div class="bw-card-sci"><em>Motacilla flava</em></div></div></div>

</div>

</details>

<!-- 02 森林公园与塔礁洲湿地 -->
<details class="bw-site" style="--accent:#5b8a52" id="forest">
<summary>02 · 森林公园与塔礁洲湿地 · Fuzhou National Forest Park &amp; Tajiangzhou Wetland <em>— Fuzhou, Fujian · 2026</em></summary>

<div class="bw-grid">

<div class="bw-card"><img src="斑鱼狗.JPG" alt="斑鱼狗 Pied Kingfisher"><div class="bw-card-body"><span class="bw-card-en">Pied Kingfisher</span><span class="bw-card-cn">斑鱼狗</span><div class="bw-card-sci"><em>Ceryle rudis</em></div></div></div>
<div class="bw-card"><img src="灰背燕尾2.JPG" alt="灰背燕尾 Slaty-backed Forktail"><div class="bw-card-body"><span class="bw-card-en">Slaty-backed Forktail</span><span class="bw-card-cn">灰背燕尾</span><div class="bw-card-sci"><em>Enicurus schistaceus</em></div></div></div>
<div class="bw-card"><img src="红嘴蓝鹊.JPG" alt="红嘴蓝鹊 Red-billed Blue Magpie"><div class="bw-card-body"><span class="bw-card-en">Red-billed Blue Magpie</span><span class="bw-card-cn">红嘴蓝鹊</span><div class="bw-card-sci"><em>Urocissa erythroryncha</em></div></div></div>
<div class="bw-card"><img src="赤红山椒鸟.JPG" alt="赤红山椒鸟 Scarlet Minivet"><div class="bw-card-body"><span class="bw-card-en">Scarlet Minivet</span><span class="bw-card-cn">赤红山椒鸟</span><div class="bw-card-sci"><em>Pericrocotus speciosus</em></div></div></div>
<div class="bw-card"><img src="铜蓝鹟.JPG" alt="铜蓝鹟 Verditer Flycatcher"><div class="bw-card-body"><span class="bw-card-en">Verditer Flycatcher</span><span class="bw-card-cn">铜蓝鹟</span><div class="bw-card-sci"><em>Eumyias thalassinus</em></div></div></div>
<div class="bw-card"><img src="长尾缝叶莺.JPG" alt="长尾缝叶莺 Common Tailorbird"><div class="bw-card-body"><span class="bw-card-en">Common Tailorbird</span><span class="bw-card-cn">长尾缝叶莺</span><div class="bw-card-sci"><em>Orthotomus sutorius</em></div></div></div>

</div>

</details>

<!-- 03 连江山堂村 -->
<details class="bw-site" style="--accent:#b07a3e" id="shantang">
<summary>03 · 连江山堂村 · Shantang Village, Lianjiang <em>— Fuzhou, Fujian · 2026</em></summary>

<div class="bw-grid">

<div class="bw-card"><img src="北红尾鸲.JPG" alt="北红尾鸲 Daurian Redstart"><div class="bw-card-body"><span class="bw-card-en">Daurian Redstart</span><span class="bw-card-cn">北红尾鸲</span><div class="bw-card-sci"><em>Phoenicurus auroreus</em></div></div></div>
<div class="bw-card"><img src="树麻雀.JPG" alt="树麻雀 Eurasian Tree Sparrow"><div class="bw-card-body"><span class="bw-card-en">Eurasian Tree Sparrow</span><span class="bw-card-cn">树麻雀</span><div class="bw-card-sci"><em>Passer montanus</em></div></div></div>
<div class="bw-card"><img src="棕背伯劳.JPG" alt="棕背伯劳 Long-tailed Shrike"><div class="bw-card-body"><span class="bw-card-en">Long-tailed Shrike</span><span class="bw-card-cn">棕背伯劳</span><div class="bw-card-sci"><em>Lanius schach</em></div></div></div>
<div class="bw-card"><img src="牛背鹭.JPG" alt="牛背鹭 Cattle Egret"><div class="bw-card-body"><span class="bw-card-en">Cattle Egret</span><span class="bw-card-cn">牛背鹭</span><div class="bw-card-sci"><em>Bubulcus ibis</em></div></div></div>
<div class="bw-card"><img src="白鹤.JPG" alt="白鹤 Siberian Crane"><div class="bw-card-body"><span class="bw-card-en">Siberian Crane</span><span class="bw-card-cn">白鹤</span><div class="bw-card-sci"><em>Leucogeranus leucogeranus</em></div></div></div>
<div class="bw-card"><img src="黑喉石鵖%20(2).JPG" alt="黑喉石鵖 Common Stonechat"><div class="bw-card-body"><span class="bw-card-en">Common Stonechat</span><span class="bw-card-cn">黑喉石鵖</span><div class="bw-card-sci"><em>Saxicola torquatus</em></div></div></div>

</div>

</details>

<!-- 04 兴化湾与闽江河口湿地 -->
<details class="bw-site" style="--accent:#7a5fa0" id="xinghua">
<summary>04 · 兴化湾与闽江河口湿地 · Xinghua Bay &amp; Minjiang Estuary Wetland <em>— Fujian · 2026</em></summary>

<div class="bw-grid">

<div class="bw-card"><img src="反嘴鹬.JPG" alt="反嘴鹬 Pied Avocet"><div class="bw-card-body"><span class="bw-card-en">Pied Avocet</span><span class="bw-card-cn">反嘴鹬</span><div class="bw-card-sci"><em>Recurvirostra avosetta</em></div></div></div>
<div class="bw-card"><img src="小天鹅.JPG" alt="小天鹅 Tundra Swan"><div class="bw-card-body"><span class="bw-card-en">Tundra Swan</span><span class="bw-card-cn">小天鹅</span><div class="bw-card-sci"><em>Cygnus columbianus</em></div></div></div>
<div class="bw-card"><img src="白琵鹭.JPG" alt="白琵鹭 Eurasian Spoonbill"><div class="bw-card-body"><span class="bw-card-en">Eurasian Spoonbill</span><span class="bw-card-cn">白琵鹭</span><div class="bw-card-sci"><em>Platalea leucorodia</em></div></div></div>
<div class="bw-card"><img src="红隼.JPG" alt="红隼 Common Kestrel"><div class="bw-card-body"><span class="bw-card-en">Common Kestrel</span><span class="bw-card-cn">红隼</span><div class="bw-card-sci"><em>Falco tinnunculus</em></div></div></div>
<div class="bw-card"><img src="鸿雁.JPG" alt="鸿雁 Swan Goose"><div class="bw-card-body"><span class="bw-card-en">Swan Goose</span><span class="bw-card-cn">鸿雁</span><div class="bw-card-sci"><em>Anser cygnoides</em></div></div></div>

</div>

</details>

<!-- Field Notes -->
<details>
<summary>Field Notes · 观鸟记录与环境思考</summary>

<div class="bw-notes">

Before I started birdwatching with my mom and an instructor from the Fujian Birdwatching Association, I had never deeply explored the natural environment around my hometown, Fuzhou. Birdwatching has given me a great opportunity to appreciate the beauty of nature and enjoy its diverse landscapes.

However, I have also noticed conflicts between human activities and wildlife. Some farmers set up bird nets around their fields to protect their crops. Meanwhile, the expansion of salt farms and industrial zones along the coast has encroached on wildlife habitats. My fellow birdwatchers have told me that both bird diversity and the number of birds we can observe have been decreasing year by year.

Humans still need to find a balance between economic development and environmental protection.

</div>

</details>

<div class="bw-acgn">

<img src="塑心壁纸1.png" alt="塑心壁纸 Virtuosa">

<em>My favorite ACGN character — Virtuosa from Arknights.</em>

</div>

</div>
</body>
</html>
