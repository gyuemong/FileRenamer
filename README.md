# File Renamer
- DLSite의 정보를 기반으로 폴더/파일명을 수정하는 프로그램(A program that renames folders and files based on information retrieved from DLsite)

## Important
- 이 도구는 사용자의 편의를 위해 개발되었으며 사용 중 데이터 손실 등의 문제가 발생할 수도 있습니다. 문제점 발견 시 건의해주시고 **중요한 파일은 반드시 사전 백업을 권장합니다.**
- This tool was developed for user convenience, but data loss or other issues may occur during use. If you encounter any problems, please report them via the issue tracker. **Always back up important files before using this tool.**

## ver1.0 기능
### 한국어
- 윈도우 환경에서만 실행 가능
- RJ넘버 혹은 VJ넘버를 통하여 DLSite에서 색인 후 해당 정보를 기반으로 폴더/파일명 변경 가능
- 내가 변환한 파일 목록에 대한 엑셀파일 내보내기 가능(현재 버전 기준 가장 마지막으로 수정된 작업 기반)
### English
- Available on Windows only  
- Allows indexing from DLsite using RJ or VJ numbers, then renames folders/files based on the retrieved information  
- Supports Excel export of converted file lists (based on the most recently modified batch in this version)  

## ver1.1 기능(사용법은 추후 수정 예정)
### 한국어
- 변경할 이름 기본값 설정
- DLSite에서 색인 시 존재하지 않는 상품 혹은 AI 상품의 경우 빠르게 다음 작업으로 넘김
- 가장 최근 작업 되돌리기 기능 추가(새로 [변경 미리보기] 버튼으로 작업 시작하는 경우 되돌리기 불가능)
- 변경할 이름에 파일 확장자가 두 번 붙는 버그 수정
### English
- Added default name format setting for renaming
- During DLSite indexing, non-existent or AI-tagged products are now quickly skipped
- Added undo function for the most recent operation  (Undo is not available if a new operation is started via the [변경 미리보기] button)
- Fixed a bug where the file extension was appended twice in the renamed filename

## 사용법
### 메인 화면
![스크린샷 2025-05-29 004114](https://github.com/user-attachments/assets/0592c726-c112-4698-82bb-da7d808d502d)
#### 한국어
1. [경로 선택] 버튼으로 변경할 폴더 및 파일들이 있는 폴더를 지정 
2. 일본어/한국어 선택으로 DLsite에서 가져올 내용의 언어를 지정 
3. 변경할 폴더 및 파일명의 양식을 설정(주의! 이미지 상의 예시 텍스트는 실제로 반영된 기본값이 아니므로 반드시 내용을 입력해야함. 디폴트는 추후 구현 예정)
4. 실제로 DLsite에서 내용을 색인한 뒤 변경할 폴더 및 파일명의 미리보기를 보여주는 기능(주의! 색인 시에 시간이 소요되는데, DLsite 내에 등록되어있지 않은 상품이 있는 경우 시간이 매우 오래 걸릴 수 있음. 추후 개선 예정)
5. 변경한 폴더 및 파일명에 해당하는 정보를 엑셀로 내보낼 수 있는 기능(가장 마지막 작업 데이터를 기준으로 내보냄) 
6. 작업 로그를 확인할 수 있는 기능(로그는 프로그램 종료 시 초기화)

#### English
1. [경로 선택] button allows you to specify the folder containing the files and directories to be renamed.
2. Choose between Japanese/Korean to determine the language of the information to be retrieved from DLsite.
3. Set the format for renaming folders and files.
   (Note: The example text shown in the image is not the actual default.
   You must enter a format manually. Default values will be implemented in a future update.)
4. After retrieving information from DLsite, the application shows a preview of the renamed folders and files.
   (Note: Indexing may take time. If the product is not registered on DLsite, it may take significantly longer. This will be improved in a future version.)
5. You can export the information of the renamed folders and files to an Excel file, based on the most recent batch of changes.
6. A log view is available to check past actions.
   (Note: Logs are cleared when the program is closed.)

### 변경 미리보기 화면
![스크린샷 2025-05-29 011355](https://github.com/user-attachments/assets/9d5dfe64-7aab-4936-9f7e-f1c85c1dfdae)
#### 한국어
1. 체크 박스로 선택된 목록만 지정한 이름 양식에 따라 변경할 수 있는 기능
2. 색인된 모든 목록을 지정한 이름 양식에 따라 변경할 수 있는 기능
3. 창 닫기

#### English
1. Allows you to rename only the items that are selected via checkboxes, using the specified naming format.
2. Allows you to rename all indexed items at once, using the specified naming format.
3. Closes the application window.

### 로그 화면
![스크린샷 2025-05-29 012155](https://github.com/user-attachments/assets/9235e30b-1aa7-49ee-960d-cd5823a60d04)
#### 한국어
1. 로그는 프로그램 종료 시 초기화되므로 [로그 내보내기] 버튼을 통해 내보낼 수 있음
#### English
1. Logs are cleared when the program is closed, but you can export them using the [로그 내보내기] button.
