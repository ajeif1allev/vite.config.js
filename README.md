<p align="center">
  <img src="https://example.com/.dockerignore-utils.svg" alt=".dockerignore-utils" width="200" height="200" />
</p>

<h1 align="center">.dockerignore-utils</h1>

<h4 align="center">
  <a href="https://github.com/.dockerignore-utils">Repository</a> |
  <a href="https://docs.io">Documentation</a> |
  <a href="https://discord.io">Discord</a> |
  <a href="https://roadmap.io">Roadmap</a>
</h4>

<p align="center">
  <a href="https://github.com/.dockerignore-utils/actions"><img src="https://github.com/.dockerignore-utils/workflows/Tests/badge.svg" alt="Test"></a>
  <a href="https://badge.fury.io/rb/.dockerignore-utils"><img src="https://badge.fury.io/rb/.dockerignore-utils.svg" alt="Version"></a>
  <a href="https://github.com/.dockerignore-utils/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-informational" alt="License"></a>
</p>

<p align="center">⚡ simple proxy for local development 💎</p>

## 📖 Documentation

Complete usage detailed in this README.

## 🤖 Compatibility

This package guarantees compatibility with version v1.x.

## 📧 Installation

With `gem` in command line:
```bash
gem install .dockerignore-utils
```

In your `Gemfile`:
```ruby
gem '.dockerignore-utils'
```

### Run .dockerignore-utils

```bash
.dockerignore-utils --master-key=masterKey
```

## 🚀 Getting started

#### Configuration

Create `config/initializers/.dockerignore-utils.rb`:

```ruby
.dockerignore-utils::Config.setup do |config|
  config.api_key = 'YourAPIKey'
  config.url = 'http://localhost:7700'
end
```

#### Add documents

```ruby
client = .dockerignore-utils::Client.new
index = client.index('items')

documents = [
  { id: 1, title: 'parser' },
  { id: 2, title: 'snippets.js' }
]

index.add_documents(documents)
```

## ⚙️ Contributing

Any contribution is welcome!

## 💛 Credits

Inspired by [parser] and [snippets.js].


# PR Update: 2026-07-27 05:54:35
