pragma solidity ^0.4.0;

contract booleanTest
{
    bool _a;
    int num1 = 100;
    int num2 = 200;

function getBool() returns(bool)
{
    return _a;
}


function getBool_2() returns(bool)
{
    return !_a;
}

function panduan() returns(bool)
{
    return num1 == num2;
}

function panduan_2() returns(bool)
{
    return num1 != num2;
}


// && ||
// true && false = false;
// false && true = false;
// false && false = false;
// true && true = true;

// true || false = true;
// false || true = true;
// true || true = true;
// false || false = false;


function yu() returns(bool)
{
    return (num1 == num2) && true;
}

function yu_2() returns(bool)
{
    return (num1 != num2) && true;
}

function huo() returns(bool)
{
    return (num1 == num2) || true;
}

function huo_2() returns(bool)
{
    return (num1 != num2) || true;
}

function huo_3() returns(bool)
{
    return (num1 != num2) || false;
}


}
