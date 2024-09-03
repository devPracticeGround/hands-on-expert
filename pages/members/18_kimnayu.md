# 안녕하세요

## 오늘 점심 메뉴 추천 목록

- 제육볶음
- 잠봉뵈르 샌드위치
- 베트남식 볶음밥

```javascript
const recommendLunchMenu = () => {
  const menuList = ['제육볶음', '잠봉', '볶음밥'];
  const randomNumber = Math.floor(Math.radnom() * 3);
  
  return menuList[randomNumber];ß
}
```