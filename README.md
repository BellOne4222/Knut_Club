[# Knut_Club
졸업작품 동아리 플랫폼
](https://github.com/Rjw510/KNUT_CLUB_Test)https://github.com/Rjw510/KNUT_CLUB_Test

1. **BoardDAO.java:**
    - **기능 설명:** 게시판 데이터베이스와 상호작용하는 DAO 클래스.
    - **중요 기능:**
        - **`updateViews(int num)`**: 특정 게시물 조회수 증가.
        - **`delNoticeAll(int[] ids)`**: 여러 공지사항 삭제.
        - **`delBoardAll(int[] ids)`**: 여러 게시물 삭제.
        - **`delNotice(int num)`**: 특정 공지사항 삭제.
        - **`delBoard(int num)`**: 특정 게시물 삭제.
        - **`getNoticeUpdate(...)`**: 공지사항 업데이트.
        - **`getBoardUpdate(...)`**: 게시물 업데이트.
        - **`getNoticeWriter(int num)`**: 특정 공지사항 작성자 조회.
        - **`getBoardWriter(int num)`**: 특정 게시물 작성자 조회.
        - **`getBoardComment(int boardNum)`**: 특정 게시물의 댓글 조회.
        - **`writeComment(...)`**: 댓글 작성.
        - **`deleteComment(int comment_num)`**: 댓글 삭제.
        - **`uploadFile(String file, int num)`**: 파일 업로드 경로 업데이트.
2. **FileStore.java:**
    - **기능 설명:** 파일 저장 및 관리를 담당하는 클래스.
    - **중요 기능:**
        - **`getFullPath(String filename)`**: 파일 전체 경로 반환.
        - **`storeFile(MultipartFile multipartFile, String domain)`**: 업로드된 파일 저장 및 정보 반환.
        - **`createStoreFileName(String originalFilename)`**: 저장할 파일 이름 생성.
3. **HomeController.java:**
    - **기능 설명:** 홈페이지의 메인 컨트롤러 클래스.
    - **중요 기능:**
        - 게시물 조회, 등록, 수정, 삭제 관련 메서드.
4. **Notice.java:**
    - **기능 설명:** 공지사항 모델 클래스.
    - **포함된 정보:**
        - 제목, 내용, 작성자, 작성일 등.
5. **Board.java:**
    - **기능 설명:** 게시물 모델 클래스.
    - **포함된 정보:**
        - 제목, 내용, 작성자, 작성일, 익명 여부 등.
6. **Comment.java:**
    - **기능 설명:** 댓글 모델 클래스.
    - **포함된 정보:**
        - 작성자, 작성일, 내용 등.

각 코드 파일은 주로 JDBC를 사용하여 MySQL 데이터베이스와 상호작용하고, Spring Framework를 활용하여 웹 애플리케이션의 핵심 기능을 구현합니다. 파일 업로드 및 관리는 **`FileStore`** 클래스에서 처리되며, 컨트롤러 클래스인 **`HomeController`**에서는 홈페이지의 주요 기능을 담당합니다.
