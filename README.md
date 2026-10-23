# 《司天考驗圖》MS.Chin.c.25：影像初錄

**v0.1.0，未獨立覆核。** 一卦 yigua.art / poplolioi11 整理。本次為非商業研究及學術資料庫利用；來源適用權利保留 CC BY-NC 4.0，整理者自有原創說明／編排採 CC BY 4.0，詳見 [LICENSE.md](LICENSE.md)。

30/30 幅完成指定文字層的第一遍影像轉錄，包含空白面判定、題名／款識、圖說、全天星圖、分宿圖、兩幅世界地圖、日月食圖、印章及館藏記號。**完整指指定範圍已逐面初錄，不是每字已辨明或全圖幾何重建；全部尚未獨立校讀或人類專家覆核。** 不作文字準確率或同儕審查主張。

## 底本與來源

清吳維鍔《司天考驗圖》不分卷，清抄本，1 冊 28×34 公分。Bodleian Libraries, University of Oxford，**MS.Chin.c.25**。館方抄本定年 1800–1899 不當成成書／出版年；精確作者生卒與首次刊行年未核。歷史作者與現代資料整理者分開。

Source credit: **MS.Chin.c.25. Photo: © Bodleian Libraries, University of Oxford.**

- [Digital Bodleian 官方物件](https://digital.bodleian.ox.ac.uk/objects/d547c5a0-f642-4dbe-92f4-6766edac9943/)
- [官方 manifest](https://iiif.bodleian.ox.ac.uk/iiif/manifest/d547c5a0-f642-4dbe-92f4-6766edac9943.json)／[館藏目錄](https://east-asian.bodleian.ox.ac.uk/catalog/volume_594)
- [館方來源授權 CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)／[利用條款](https://digital.bodleian.ox.ac.uk/terms/)（2026-10-23 查核）

原 manifest 的 30 幅順序與館方葉標保留，包括 `fol. (10a)a`、`fol. (10a)b` 插葉。不把畫布數當葉數或文字頁數；空白面為 c002, c003, c004, c028, c029, c030。背面透字不重複計成該面正文。逐幅來源與工作圖 hash 見 [source-index.json](source-index.json)，詳情見 [PROVENANCE.md](PROVENANCE.md)。

## 檔案與資料結構

- [transcription.txt](transcription.txt)：可直接閱讀；方括號導覽、角色及定位為現代新增，非原書正文。
- [transcription.json](transcription.json)：依畫布、文字區塊與圖形記錄來源、原文、座標、疑字與限制。
- [transcription.tei.xml](transcription.tei.xml)：與 JSON 文字區塊原文一致的 TEI P5；surface/zone 保留來源與座標，ab 保留文字並連到 figure，figDesc 是現代描述。來源、圖形及疑字（含 extent）以對應 note 保存；完整資料仍以配套 JSON 為準。
- [uncertainties.json](uncertainties.json)：124 筆定位疑字，正文中的 `□` 共 124 個；字數未詳文段另記 extent，不能把占位數直接當缺字數或錯誤率。
- [source-index.json](source-index.json)、[SHA256SUMS](SHA256SUMS)、[CITATION.cff](CITATION.cff)、[VALIDATION.json](VALIDATION.json)：來源、校驗、引用與驗證範圍。

共 1414 個文字區塊與 36 個現代圖形描述。`bbox=[x,y,width,height]` 是實際工作影像像素；文字位置從 1 起算 Unicode 碼點。正文直欄按原版式，圖內標籤按空間位置另列，不虛構連續語句。圖形幾何、星點、海岸線及經緯網線未重建。

不自動加標點、統一異體或簡繁轉換。不用通行本、地理常識或模型記憶代填原頁。這仍可能有漏讀、錯讀或版式誤判；關鍵引文與研究統計應回到原圖核對。AI 輔助初錄的模型／方法與覆核界線詳 PROVENANCE；未提供私人處理程式、提示、工作影像或完整 AI 工作紀錄，不宣稱全流程可重跑。

## 驗證與覆核

已核 30 幅來源位元組 hash、頁序／ID、座標範圍、圖形標籤對應、逐一疑字位置、JSON/TXT/TEI 文字回讀一致性及官方 TEI P5 4.12.0 Relax NG。另做改字、掉區塊、換序、錯來源、疑字錯位、重複ID與外部entity的拒絕測試；CFF依完整官方1.2.0 schema驗證。

未執行獨立影像盲校、人類專家覆核、逐字準確率量測、完整異文校勘、ODD或Schematron。格式及 hash 只驗所聲明的一致性，不證明讀字正確、學術認證或法律認證。

## 引用與訂正

版本 DOI：[10.5281/zenodo.23588495](https://doi.org/10.5281/zenodo.23588495)（製備時已預留；正式發布／登記以平台公開紀錄為準）。

請分開引用：① 吳維鍔《司天考驗圖》與相應葉／區塊；② Bodleian MS.Chin.c.25 官方影像；③ 一卦 yigua.art / poplolioi11（2026），本資料 v0.1.0（影像初錄，未獨立覆核）。固定發行版：https://github.com/poplolioi11/ms-chin-c25-sitian-kaoyantu/releases/tag/v0.1.0 。

Issues 歡迎附原頁證據的訂正，方式見 [CONTRIBUTING.md](CONTRIBUTING.md)。改字另發版本，保留原版本與變更，不默換封存檔。CFF及DOI不會追蹤所有使用或引用。

## English summary

An AI-assisted first-pass transcription of *Si tian kao yan tu*, attributed to Wu Wei'e, from Bodleian MS.Chin.c.25. All 30 canvases were inspected for the specified text layer, including chart and map labels, paratext and blank surfaces. Uncertainties remain; there has been no independent collation or human expert review. Geometry is not reconstructed. JSON, TXT and TEI retain page/region source alignment. Source applicable rights remain CC BY-NC 4.0 for noncommercial scholarly use; original documentation and arrangement are CC BY 4.0. These are distinct rights layers, not a choice of licences for the whole package. Scans and private processing materials are excluded. Please cite the historical author, source manuscript and this versioned dataset separately.
