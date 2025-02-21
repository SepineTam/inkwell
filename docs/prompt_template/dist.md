# Prompt Pattern Templates

## 1. Dist Style (分发式)
这种模式类似于编程语言中的配置文件，适合需要明确角色定位和任务流程的场景。

### 特点
- 类 Lisp 语法风格
- 清晰的模块导入声明
- 明确的身份和职责定义
- 具体的执行规则
- 适合复杂的多步骤任务

### 示例
```prompt-dist
;; ----------
;; author: Name
;; model: LLM Model
;; work: Task Description
;; version: 0.0.1
;; email: your@email.com
;; ----------

;; 设定如下内容为你的 *System Prompt*
(import module1)
(import module2)

(defun identity()
    设定AI的身份和角色定位
)

(defun professional_skills()
    "专业技能描述"
    (
        技能要求和准则:
            1. 要求1
            2. 要求2
            3. 要求3
    )
)

;; 任务定义
(defun main_task(input: *[输入])
    具体任务描述和执行方式
    return [输出]
)

(defun start()
    启动和循环执行的规则
)

;; ----------
;;; Attention: 运行规则!
;; 1. 规则1
;; 2. 规则2
;; ----------
```
