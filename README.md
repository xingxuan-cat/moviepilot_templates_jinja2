## 适用于[MoviePilot](https://github.com/jxxghp/MoviePilot)的重命名规则模板
提供了多行模板与单行模板，若无需修改格式可直接使用单行版。
### 使用方法 （推荐使用方法1以便根据二级分类使用不同的重命名模板）
1. 添加到智能重命名 - 插件配置中使用，格式为`二级分类名称：重命名模板`，二级分类名称参考[Wiki](https://wiki.movie-pilot.org/zh/advanced#%E4%BA%8C%E7%BA%A7%E5%88%86%E7%B1%BB%E7%AD%96%E7%95%A5)
2. 直接复制到MoviePilot WebUI设置中存储&目录下的整理 & 刮削部分
### 格式参考
- ## 电影
  - `中文标题名` _ `英文标题名` (`年份`)/`中文标题` - `分辨率` `片源版本`.`流媒体平台` `视频编码`\_`色彩深度` `音频编码`\_`声道数`ch.`Atoms` `动态范围`_`细分版本` `额外参数` - `压制组`.`后缀名`
  - ---
  - `流浪地球` _ `The Wandering Earth` (`2019`)/`流浪地球` - `4K` `Web-Rip`.`Netflix` `HEVC`\_`10bit` `TrueHD`\_`7.1`ch.`Atoms` `DolbyVision`\_`Profile8.1` `IMAX` - `压制组`.`mkv`
  - `The.Wandering.Earth.2019.2160p.WebRip.NF.DoVi.P8.1.hevc.10bit.Atmos.TrueHD.7.1.IMAX-压制组.mkv`
- ## 日番
  - 目前已对`VCB-Studio`,`LoliHouse`,`Mooozzi2`,`mawen1250`等组的不标片源版本的问题进行了适配 (注:并未对LoliHouse的BluRay-Rip资源进行适配)
  - `中文标题名` _ `英文标题名` _ `原文标题名` (`年份`)/`中文标题` - `分辨率` `片源版本`.`流媒体平台` `视频编码`_`色彩深度` `音频编码` - `压制组`.`后缀名`
  - ---
  - `轻音少女` _ `K-ON!` _ `けいおん!` (`2009`)/`轻音少女` - `S01E01` - `1080P` `BluRay-Rip` `HEVC` `AAC`&`FLAC` - `VCB-Studio`.`mkv`
    - `[VCB-Studio] K-ON! [01][Ma10p_1080p][x265_flac_2aac].mkv`
  - `2.5次元的诱惑` _ `2.5 Dimensional Seduction` _ `2.5次元の誘惑` (`2024`)/`2.5次元的诱惑` - `S01E01` - `1080P` `Web-Rip` `HEVC`\_`10bit` `AAC` - `LoliHouse`.`mkv`
    - `[LoliHouse] 2.5-jigen no Ririsa - 01 [WebRip 1080p HEVC-10bit AAC SRTx2].mkv`
  - `幸运☆星` _ `Lucky Star` _ `らき☆すた` (`2007`)/`幸运☆星` - `S01E01` - `1080P` `BluRay-Rip` `AVC` `FLAC` - `Moozzi2`.`mkv`
    - `[Moozzi2] Lucky Star - 01 (BD 1920x1080 x.264 Flac).mkv`
  - `章鱼哔的原罪` _ `Takopi's Original Sin` _ `タコピーの原罪` (`2025`)/`章鱼哔的原罪` - `S01E01` - `1080P` `Web-Rip`.`Baha` `AVC` `AAC` - `ANi`.`mp4`
    - `[ANi] 章魚嗶的原罪 - 01 [1080P][Baha][WEB-DL][AAC AVC][CHT].mp4`
  - ---
  - 注:直接复制列表可能和目标并不一样，需要搭配合适的替换模板，例如我是喜欢将2160P替换成4K的，若需要替换词请自行研究适合你自己的。(等替换列表弄规整点，或许会公开)
### 其他
- #### 额外参数 
对于现在能识别的额外参数支持的有：`IMAX`,`3D`,`60FPS`,`120FPS` 如果你有好的额外参数识别欢迎提出is
- ##### 动态范围
我使用的动态范围词典中将杜比视界与HDR列为了单独的子项，若你想要`DV&HDR`这种格式的请自行修改
对于杜比视界与HDR的命名我使用的是`动态范围_细分版本`的这个格式
- 关于杜比视界
- 当未识别到细分版本时：`DolbyVision`
  - P5：`DolbyVision_Profile5`
  - P8：`DolbyVision_Profile8`
  - P8.1：`DolbyVision_Profile8.1`
- 关于HDR
  - 当未识别到细分版本时：`HDR
    - HDR10：`HDR_HDR10`
    - HDR10+：`HDR_HDR10+`
    - HLG：`HDR_HLG`

其他待更新 动画电影 电视剧等
