## Title
Thank you for attending this presentation.
Today, I would like to talk to you about "Beginner’s guide to Flutter with DDD"

## Self Intoroduction
At first, let me introduce myself.
My name is Masataka Ushijima and I am software engineer.
I work at Leverages, HR company in Tokyo, Japan.
Recently I have made native app with flutter in my job.
In my free time, I like traveling around the world, training, and customize notion.
I lived in gaogao tokyo until 03/2020.

## Today's topic
So, Today's topic is flutter with DDD.
I began to learn about flutter with ddd two month ago.
Today, I would like to show my knowledge I got in two month.

## What's Flutter
At first, What is flutter.
In official site, There is sentence,
"Flutter is Google's UI toolkit for building beautiful,
natively compiled applications for mobile, web,
and desktop from a single codebase"

it means flutter is toolkit for making native app.

the merit of using flutter are
- fast development, for example, you can use hot reload
- expressive, beautiful UI
- native performance

## What's Dart
so, next, what's dart.

in official site. there is sentence
"Dart is client-optimized language for performance fast apps on any platform."

the merit of using dart are
- optimize for UI
- productive development
- fast on all platforms
- OOP like JS

if you use dart with flutter, you can make native apps fastly.
today's topic is DDD, so if you want to know about dart and flutter,
let's visit official site. it's very undarstandable.

## How to develop with Flutter
initial directory like this.
we write code in lib directory mainly.
in this directory, you can make directory and files freely.
when using ddd, you should make them in this directory.

when you compile files, you can use app in ios, android, web.

## what' ddd
DDD is the process to design software with Object oriented programming.
it is almost Object oriented design.
there are a lot of concept like this.

and we can choose architecture from these architecture.

and I think architecture easy to use for begineer is onionarchitecture

because
- simple directory architecture for begineer
- a lot of useful infomation on website

this is onion architecture
domain is center
presentation, infrastructure depends application, and application depends domain. it's unidirectional.

## Directory structure
in my flutter project, directory structure like this.
I would like to introduce this structure.

call flow from presentation
ui calls notifier
and notifier calls application service
and application service calls domain service and domain service calls repository

data flow from sqlight and firebase
infrastructure implements repository and called by domain service

lets see this in detail

at first application
there are two directory
dto is making data object for ui
service is usecase

domain
there are two directory
model includes entity, repository and value object
service is domain service

infrastructure
there are three directory 
getit for di container, make repository object as singleton
repository is detail repository implementation
sqflight is setting swlight database


presentation
there are two directory
notifier is for managing state directory
ui is view directory with atomic design


## Pros and Cons

## thank you
This is all for my presentation.
thank you.