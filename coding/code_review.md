# 代码审查建议生成

## 提示词

```
我需要对以下{编程语言}代码进行代码审查。请帮我分析可能存在的问题，包括但不限于：代码质量、性能优化、安全隐患、可维护性、最佳实践等。请提供具体的改进建议，并说明原因。

```代码
{在这里粘贴代码}
```
```

## 示例

```
我需要对以下JavaScript代码进行代码审查。请帮我分析可能存在的问题，包括但不限于：代码质量、性能优化、安全隐患、可维护性、最佳实践等。请提供具体的改进建议，并说明原因。

```javascript
function getData(userInput) {
  // 从API获取数据
  var apiUrl = 'https://api.example.com/data?q=' + userInput;
  var result = fetch(apiUrl)
    .then(function(response) {
      return response.json();
    })
    .then(function(data) {
      return data;
    });
  
  return result;
}

// 处理用户提交
function handleSubmit() {
  var input = document.getElementById('userInput').value;
  getData(input).then(function(data) {
    document.getElementById('result').innerHTML = data.name + ' is ' + data.age + ' years old.';
  });
}
```
```

## 说明

这个提示词用于获取专业的代码审查意见，有助于提高代码质量和发现潜在问题。适用于各种编程语言的代码审查需求。