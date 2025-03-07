# solution-homework-4

Overview

This project demonstrates the implementation of two important structural design patterns in Java:
Singleton Pattern – A Global Configuration Manager.
Adapter Pattern – A Chat Service Adapter that integrates a legacy chat system into a modern interface.

Singleton Pattern:

Objective

Ensure that only one instance of a configuration manager exists throughout the application, providing a centralized, globally accessible resource.

Implementation Details

The ConfigurationManager class follows the Singleton pattern.
Stores configuration values in a hardcoded key-value pair format.
Uses lazy initialization to create an instance only when needed.
Provides methods to retrieve values and print all configurations.

Files

ConfigurationManager.java – Implements the Singleton pattern.
ConfigManagerDemo.java – Demonstrates retrieving and printing configurations.

Output:

maxPlayers: 100

defaultLanguage: en

gameDifficulty: medium

All Configurations:

maxPlayers → 100

defaultLanguage → en

gameDifficulty → medium

Adapter Pattern:

Objective

Enable integration of a legacy chat system with our application by adapting its interface to the expected format.

Implementation Details

The ChatServiceAdapter wraps around LegacyChatService and translates calls.
Ensures the legacy system's sendLegacyMessage() can be accessed via the ChatService interface.

Files

ChatService.java – Defines the target interface.
LegacyChatService.java – Simulates the old chat service.
ChatServiceAdapter.java – Implements the adapter to translate messages.
ChatAdapterDemo.java – Demonstrates sending a message via the adapter.

Output:

Legacy Chat: Hello world!
