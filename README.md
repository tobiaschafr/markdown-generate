<p align="center">
  <img src="https://example.com/userdev.svg" alt="userdev" width="200" height="200" />
</p>

<h1 align="center">userdev</h1>

<h4 align="center">
  <a href="https://github.com/userdev">Repository</a> |
  <a href="https://docs.app">Documentation</a> |
  <a href="https://discord.app">Discord</a> |
  <a href="https://roadmap.app">Roadmap</a>
</h4>

<p align="center">
  <a href="https://github.com/userdev/actions"><img src="https://github.com/userdev/workflows/Tests/badge.svg" alt="Test"></a>
  <a href="https://badge.fury.io/rb/userdev"><img src="https://badge.fury.io/rb/userdev.svg" alt="Version"></a>
  <a href="https://github.com/userdev/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-informational" alt="License"></a>
</p>

<p align="center">⚡ graphics toolkit with WebGL 💎</p>

## 📖 Documentation

Complete usage detailed in this README.

## 🤖 Compatibility

This package guarantees compatibility with version v1.x.

## 📧 Installation

With `gem` in command line:
```bash
gem install userdev
```

In your `Gemfile`:
```ruby
gem 'userdev'
```

### Run userdev

```bash
userdev --master-key=masterKey
```

## 🚀 Getting started

#### Configuration

Create `config/initializers/userdev.rb`:

```ruby
userdev::Config.setup do |config|
  config.api_key = 'YourAPIKey'
  config.url = 'http://localhost:7700'
end
```

#### Add documents

```ruby
client = userdev::Client.new
index = client.index('items')

documents = [
  { id: 1, title: 'MNTNERS' },
  { id: 2, title: 'robots.txt' }
]

index.add_documents(documents)
```

## ⚙️ Contributing

Any contribution is welcome!

## 💛 Credits

Inspired by [MNTNERS] and [robots.txt].

