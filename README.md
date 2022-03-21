# 키친포스

## 요구 사항

### 상품

- 상품을 등록할 수 있다.
- 상품의 가격이 올바르지 않으면 등록할 수 없다.
  - 상품의 가격은 0원 이상이어야 한다.
- 상품의 이름이 올바르지 않으면 등록할 수 없다.
  - 상품의 이름에는 비속어가 포함될 수 없다.
- 상품의 가격을 변경할 수 있다.
- 상품의 가격이 올바르지 않으면 변경할 수 없다.
  - 상품의 가격은 0원 이상이어야 한다.
- 상품의 가격이 변경될 때 메뉴의 가격이 메뉴에 속한 상품 금액의 합보다 크면 메뉴가 숨겨진다.
- 상품의 목록을 조회할 수 있다.

### 메뉴 그룹

- 메뉴 그룹을 등록할 수 있다.
- 메뉴 그룹의 이름이 올바르지 않으면 등록할 수 없다.
  - 메뉴 그룹의 이름은 비워 둘 수 없다.
- 메뉴 그룹의 목록을 조회할 수 있다.

### 메뉴

- 1 개 이상의 등록된 상품으로 메뉴를 등록할 수 있다.
- 상품이 없으면 등록할 수 없다.
- 메뉴에 속한 상품의 수량은 0 이상이어야 한다.
- 메뉴의 가격이 올바르지 않으면 등록할 수 없다.
  - 메뉴의 가격은 0원 이상이어야 한다.
- 메뉴에 속한 상품 금액의 합은 메뉴의 가격보다 크거나 같아야 한다.
- 메뉴는 특정 메뉴 그룹에 속해야 한다.
- 메뉴의 이름이 올바르지 않으면 등록할 수 없다.
  - 메뉴의 이름에는 비속어가 포함될 수 없다.
- 메뉴의 가격을 변경할 수 있다.
- 메뉴의 가격이 올바르지 않으면 변경할 수 없다.
  - 메뉴의 가격은 0원 이상이어야 한다.
- 메뉴에 속한 상품 금액의 합은 메뉴의 가격보다 크거나 같아야 한다.
- 메뉴를 노출할 수 있다. (전시)
- 메뉴의 가격이 메뉴에 속한 상품 금액의 합보다 높을 경우 메뉴를 노출할 수 없다.
- 메뉴를 숨길 수 있다.
- 메뉴의 목록을 조회할 수 있다.

### 주문 테이블 (식탁)

- 주문 테이블을 등록할 수 있다.
- 주문 테이블의 이름이 올바르지 않으면 등록할 수 없다.
  - 주문 테이블의 이름은 비워 둘 수 없다.
- 빈 테이블을 해지할 수 있다.
- 빈 테이블로 설정할 수 있다.
- 완료되지 않은 주문이 있는 주문 테이블은 빈 테이블로 설정할 수 없다.
- 방문한 손님 수를 변경할 수 있다.
- 방문한 손님 수가 올바르지 않으면 변경할 수 없다.
  - 방문한 손님 수는 0 이상이어야 한다.
- 빈 테이블은 방문한 손님 수를 변경할 수 없다.
- 주문 테이블의 목록을 조회할 수 있다.

### 주문

- 1개 이상의 등록된 메뉴로 배달 주문을 등록할 수 있다.
- 1개 이상의 등록된 메뉴로 포장 주문을 등록할 수 있다.
- 1개 이상의 등록된 메뉴로 매장 주문을 등록할 수 있다.
- 주문 유형이 올바르지 않으면 등록할 수 없다.
- 메뉴가 없으면 등록할 수 없다.
- 매장 주문은 주문 항목의 수량이 0 미만일 수 있다.
- 매장 주문을 제외한 주문의 경우 주문 항목의 수량은 0 이상이어야 한다.
- 배달 주소가 올바르지 않으면 배달 주문을 등록할 수 없다.
  - 배달 주소는 비워 둘 수 없다.
- 빈 테이블에는 매장 주문을 등록할 수 없다.
- 숨겨진 메뉴는 주문할 수 없다.
- 주문한 메뉴의 가격은 실제 메뉴 가격과 일치해야 한다.
- 주문을 접수한다. (수락)
- 접수 대기 중인 주문만 접수할 수 있다.
- 배달 주문을 접수되면 배달 대행사를 호출한다.
- 주문을 서빙한다. (조리 완료)
- 접수된 주문만 서빙할 수 있다.
- 주문을 배달한다.
- 배달 주문만 배달할 수 있다.
- 서빙된 주문만 배달할 수 있다.
- 주문을 배달 완료한다.
- 배달 중인 주문만 배달 완료할 수 있다.
- 주문을 완료한다.
- 배달 주문의 경우 배달 완료된 주문만 완료할 수 있다.
- 포장 및 매장 주문의 경우 서빙된 주문만 완료할 수 있다.
- 주문 테이블의 모든 매장 주문이 완료되면 빈 테이블로 설정한다.
- 완료되지 않은 매장 주문이 있는 주문 테이블은 빈 테이블로 설정하지 않는다.
- 주문 목록을 조회할 수 있다.

## 용어 사전

| 한글명   | 영문명              | 설명                                                                                  |
|-------|------------------|-------------------------------------------------------------------------------------|
| 상품    | Product          | 메뉴 상품을 구성하는 음식이다. 가격은 0원 이상이다.                                                      | 
| 메뉴 그룹 | MenuGroup        | 메뉴의 공통적인 특성을 묶은 대분류.                                                                |
| 메뉴    | Menu             | 키친 포스에서 판매하는 상품의 묶음. 하나일 수도 묶음일 수도 있다. 상품 묶음의 합산 가격보다 같거나 낮아야 한다.                   |
| 전시    | Display          | 판매할 수 있는 메뉴의 상태. 숨길 수 있다.                                                           |
| 숨김    | Hide             | 판매할 수 없는 메뉴의 상태. 전시할 수 있다.                                                          |
| 메뉴 상품 | Menu Product     | 메뉴를 구성하는 각각의 상품과 수량.                                                                |
| 식탁    | Order Table      | 매장 주문 시 고객이 식사를 할 수 있는 곳으로 비어있지 않은 상태에서만 주문이 가능하다.                                  |
| 고객    | Guest            | 메뉴를 주문하는 사람.                                                                        |
| 주문    | Order            | 고객이 메뉴를 구입하는 행위.                                                                    |
| 주문 항목 | Order Line Item  | 고객이 주문하고자 하는 각각의 메뉴의 수량과 가격.                                                        |
| 배달 주문 | Delivery Order   | 판매자가 음식을 배달대행사 전달하여 고객에게 전달하는 주문이다. 주문 상태는 대기, 접수, 조리 완료, 배달 중, 배달 완료, 완료 순서로 진행된다. |
| 포장 주문 | TAKE-OUT Order   | 판매자가 고객에게 직접 전달하는 주문이다. 주문 상태는 대기, 접수, 조리 완료, 완료 순서로 진행된다.                          |
| 매장 주문 | EAT-IN Order     | 판매자가 식탁으로 음식을 전달하는 주문이다. 주문 상태는 대기, 접수, 조리 완료, 완료 순서로 진행된다.                         |
| 배달대행사 | Delivery Service | 배달 주문 시 음식을 고객에게 전달하는 외부 업체.                                                        |
| 대기    | WAITING          | 주문의 최초 상태. 모든 주문이 가질 수 있는 상태이다.                                                     |
| 수락    | ACCEPTED         | 조리 가능할 경우 변경되는 주문의 상태. 대기 중인 주문에서만 수락할 수 있다.                                        |
| 조리 완료 | SERVED           | 수락된 주문의 음식이 고객에게 전달 가능한 상태인 경우 변경되는 주문의 상태. 수락된 주문만 조리할 수 있다.                       |
| 배달 중  | DELIVERING       | 조리 완료된 주문의 음식이 고객에게 배달하기 위해 배달대행사에게 전달된 경우 변경되는 주문의 상태. 조리 완료된 배달 주문만 배달할 수 있다.     |
| 배달 완료 | DELIVERED        | 배달대행사가 고객에게 음식을 전달한 경우 변경되는 주문의 상태. 배달 중인 배달 주문만 배달 완료할 수 있다.                       |
| 완료    | COMPLETED        | 주문이 전부 완료된 경우 변경되는 주문의 상태. 조리 완료 또는 배달 완료된 주문만 완료할 수 있다.                            |


## 모델링
