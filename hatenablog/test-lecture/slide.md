---
title: Androidテスト基礎講義
marp: true
theme: default
paginate: true
---

# Androidテスト基礎講義

---

## 1. はじめに
- Android開発におけるテストの重要性
- 今後の開発業務でなぜテストが必要か

---

## 2. Androidテストの全体像
- テストの種類
  - ユニットテスト（Unit Test）
  - インストルメンテーションテスト（Instrumented Test）
  - UIテスト（Espressoなど）
- テストのピラミッド
  - 単体テスト、統合テスト、UIテストのバランス

---

## テストの種類
| 種類 | 実行環境 | 目的 |
|------|----------|------|
| ユニットテスト | JVM | ロジックの検証 |
| インストルメンテーションテスト | 実機/エミュレータ | Android APIの検証 |
| UIテスト | 実機/エミュレータ | 画面操作の自動化 |

---

## 3. ユニットテストの基礎
- ユニットテストとは
- JUnitの基本
  - テストクラス・メソッドの書き方
  - アサーションの使い方
- モック（Mockitoなど）の活用
- サンプルコード紹介

---

### JUnitによるユニットテスト例
```kotlin
class CalculatorTest {
    @Test
    fun add_isCorrect() {
        assertEquals(4, Calculator.add(2, 2))
    }
}
```

---

## 4. インストルメンテーションテストとUIテスト
- インストルメンテーションテストとは
  - 実機やエミュレータ上でのテスト
- UIテストの自動化
  - Espressoの概要
  - テストケースの例
- テストの実行方法（Android Studioでの実演）

---

### EspressoによるUIテスト例
```kotlin
@Test
fun testButtonClick() {
    onView(withId(R.id.button)).perform(click())
    onView(withId(R.id.textView)).check(matches(withText("Hello")))
}
```

---

## 5. テストの実践とベストプラクティス
- テストコードの管理
- テストの命名規則
- CI/CDとの連携
- よくある失敗例とその対策

---

## ベストプラクティス
- 小さく書く、頻繁に実行する
- テストの失敗はすぐ直す
- レビュー時にテストも確認

---

## 6. まとめ・質疑応答
- 本日のまとめ
- 参考ドキュメントの紹介
  - [Android公式テストガイド](https://developer.android.com/training/testing)
  - [テストの基礎](https://developer.android.com/training/testing/fundamentals)
  - [Android Studioでのテスト](https://developer.android.com/studio/test/test-in-android-studio)
- 質疑応答 