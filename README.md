# 《司天考驗圖》MS.Chin.c.25：獨立 AI 二校

**v0.2.0，保留疑字；未經人類專家審定。** 整理者：曲宸宇（Chu, Chen-Yu；GitHub：poplolioi11；[ORCID](https://orcid.org/0009-0003-9738-6914)）。

本版對全書30幅的指定文字層與全頁版面作另一次獨立影像讀字、比較及回圖裁決，涵蓋題名、款識、星圖標籤、圖說韻文與占辭、兩幅世界地圖、日月食圖、印記、館藏記號及空白面。可用於名稱索引、來源定位及後續校勘；正式引用韻文、占辭或疑字，請核對原圖與疑字記錄。這不是人類雙校、專家定本或準確率認證。

## 底本與範圍

清吳維鍔《司天考驗圖》，Bodleian Libraries, University of Oxford，**MS.Chin.c.25**。館方抄本編目年代1800–1899不當作成書或出版年。30個IIIF畫布按館方原序保存，不能當作30葉；空白面為c002、c003、c004、c028、c029、c030。

[Digital Bodleian官方影像](https://digital.bodleian.ox.ac.uk/objects/d547c5a0-f642-4dbe-92f4-6766edac9943/) · [官方manifest](https://iiif.bodleian.ox.ac.uk/iiif/manifest/d547c5a0-f642-4dbe-92f4-6766edac9943.json) · [正式書目](https://east-asian.bodleian.ox.ac.uk/catalog/volume_594)

Source credit: **MS.Chin.c.25. Photo: © Bodleian Libraries, University of Oxford.** 影像不隨本包散布。來源適用權利保留[CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)；整理者自有說明與原創編排另採[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)，兩者分層適用，詳[LICENSE.md](LICENSE.md)。

## 本版內容

本版有1410個文字區塊、311筆定位疑讀，正文中有101個`□`。疑讀記錄也可能標在已錄出的字上；一個`□`可代表字數未定的片段，不能將這些數量當成缺字數、錯誤率或準確率。圖形仍是36個現代描述，星點、連線、海岸線與經緯網幾何未重建。

相較固定v0.1.0，335個既有區塊文字有變動、移除20個誤框／重複單位、新增16個來源單位。這些是區塊級變動數，包含分組與原寫字形訂正，不等於錯字數。逐項見[corrections.json](corrections.json)、[region-mapping.json](region-mapping.json)與[COLLATION.md](COLLATION.md)。

- [TXT](transcription.txt)：直接閱讀。方括號導覽與角色標籤是現代新增，非原文。
- [JSON](transcription.json)：主資料，保存來源、原文、角色、近似文字框、疑字及覆核狀態。
- [TEI P5 XML](transcription.tei.xml)：與JSON逐區塊文字一致；surface/zone、ab、figure與疑字note保留來源對應。完整資料以配套JSON為準。
- [疑字](uncertainties.json)、[來源與官方高解析影像區域](source-index.json)、[覆核摘要](collation-report.json)、[格式驗證](VALIDATION.json)、[校驗值](SHA256SUMS)、[引用](CITATION.cff)。

`bbox=[x,y,width,height]`用固定工作影像的實際像素；文字位置從1起算Unicode碼點。文字框是近似定位或讀取鄰域，可能包含鄰字，不是精密字界、星點座標或量測資料。圖中名稱按位置另錄，不拼成虛構連續語句。

## 覆核與限制

獨立讀字先於兩稿比較；有差異、疑字與列明高風險項再回圖裁決。星官術語及《步天歌》詞例用於提出疑問，不能取代底本筆形。不自動補標點、統一異體、正規化地名、修正底本本身可能的訛寫；來源不可唯一辨讀時，保留候選與理由。

本輪使用Codex影像工作者（要求gpt-6-astra、ultra；實際逐次服務模型未獨立回報）及AI Coop的Gemini影像工作（回報gemini-3.8-flash-high）。程式只處理確定規則的比對、編碼、雜湊與一致性檢查。沒有做人類專家審定、同儕審查、人工參考逐字準確率量測或完整異本校勘。詳[PROVENANCE.md](PROVENANCE.md)。

JSON/TXT/TEI回讀、頁序、ID、來源雜湊、文字框範圍、疑字定位、官方TEI Relax NG及完整CFF 1.2.0 schema另作驗證。這些驗證不證明文字無誤。專用程式、提示、裁片及完整協作紀錄私人保存，未提供由原圖完全重跑辨字的方法。

## 引用、版本與訂正

本版的 Zenodo 版本 DOI 尚未建立；請先以固定 GitHub v0.2.0 連結引用。以下全版本 DOI 目前仍指向舊版，不能用來代表本次二校。 [全版本DOI](https://doi.org/10.5281/zenodo.23588494) · [GitHub固定v0.2.0](https://github.com/poplolioi11/ms-chin-c25-sitian-kaoyantu/releases/tag/v0.2.0)。

Chu, Chen-Yu（曲宸宇）. (2026). 《司天考驗圖》MS.Chin.c.25：獨立 AI 二校（保留疑字）, v0.2.0.

研究引用請另列歷史作者、Bodleian底本與具體畫布／區塊。v0.1.0初錄、舊tag、檔案與[舊版DOI](https://doi.org/10.5281/zenodo.23588495)均保留。新版不回寫舊版。歡迎在[Issues](https://github.com/poplolioi11/ms-chin-c25-sitian-kaoyantu/issues)附原頁證據訂正，見[CONTRIBUTING.md](CONTRIBUTING.md)。

## English summary

An independently collated AI transcription of *Si tian kao yan tu*, attributed to Wu Wei'e, Bodleian MS.Chin.c.25. All declared text layers and page layouts across 30 canvases were reviewed, including star-chart and world-map labels, captions, prognostications, eclipse diagrams and paratext. Unresolved readings are explicitly retained. There has been no human expert review or measured character-accuracy evaluation. This is a provisional source-aligned research aid; verify quotations against the manuscript images. Geometry is not reconstructed. Source applicable rights remain CC BY-NC 4.0; original documentation and arrangement are separately CC BY 4.0. Scans and private processing materials are excluded.
