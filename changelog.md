# Changelog
All updates to the Ryujinx official master build will be documented in this file

## 1.0.4697 - 2020-06-14
### Fixed
- Fixed an issue where part of the VABS instruction would be parsed as an input register.
- Fixed particular DEADLY PREMONITION Origins missing opcode error; the instruction was not missing but was instead parsed incorrectly. 

## 1.0.4696 - 2020-06-14
### Changed
- LayoutConverter has separate optimizations for LinearStrided and BlockLinear. MethodCopyBuffer now determines the range that will be affected, and uses a faster per pixel copy and offset calculation.
- Increases performance on Nintendo Switch Online: NES and Super NES games.
- Mitigates dropped frames during large black screen (nvdec) videos.
