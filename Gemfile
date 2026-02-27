source "https://rubygems.org"
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

ruby "3.2.9"

# Rails本体
gem "rails", "~> 7.1.0"
gem "bcrypt", "~> 3.1.18"


# 基本機能
gem "sprockets-rails", "3.4.2"  # ← バージョンを指定
gem "bootstrap-sass", "3.4.1"   # ← これを追加！
gem "sassc-rails", "2.1.2"      # ← これも追加！
gem "puma", ">= 5.0"
gem "importmap-rails"
gem "turbo-rails"
gem "stimulus-rails"
gem "jbuilder"
gem "bootsnap", require: false

# 開発・テスト環境（SQLite3を使う）
group :development, :test do
  gem "sqlite3", "~> 1.4"
  gem "debug", platforms: %i[ mri mingw x64_mingw ]
end

# 開発環境のみ
group :development do
  gem "web-console"
  gem "guard"
end

# テスト環境のみ
group :test do
  gem "capybara"
  gem "selenium-webdriver"
  gem "minitest", "< 6.0"
  gem "guard-minitest"
  gem "minitest-reporters", ">= 1.0.5"
  gem 'rails-controller-testing'
end

# 本番環境（Render用：Postgresを使う）
group :production do
  gem "pg"
end

# Render restart trigger