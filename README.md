# -yuxin-.github.io
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>布行财务管理系统 | 高端面料财务解决方案</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css"  rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css"> 
    <style>
        :root {
            --primary: #5c6bc0;
            --secondary: #7e57c2;
            --accent: #26a69a;
            --dark: #263238;
            --light: #f5f5f5;
        }
        
        body {
            font-family: 'Helvetica Neue', Arial, sans-serif;
            background-color: #f8fafc;
        }
        
        .table-container {
            box-shadow: 0 10px 30px -15px rgba(0, 0, 0, 0.1);
            border-radius: 12px;
            overflow: hidden;
        }
        
        .table-header {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
        }
        
        .input-field {
            transition: all 0.3s ease;
            border-radius: 6px;
        }
        
        .input-field:focus {
            box-shadow: 0 0 0 3px rgba(92, 107, 192, 0.3);
        }
        
        .btn-primary {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            transition: all 0.3s ease;
        }
        
        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(92, 107, 192, 0.4);
        }
        
        .btn-secondary {
            background: var(--accent);
            transition: all 0.3s ease;
        }
        
        .btn-secondary:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(38, 166, 154, 0.4);
        }
        
        .highlight-row {
            transition: all 0.3s ease;
        }
        
        .highlight-row:hover {
            background-color: rgba(92, 107, 192, 0.05);
        }
        
        .tab-active {
            border-bottom: 3px solid var(--primary);
            font-weight: 600;
            color: var(--primary);
        }
        
        .fade-in {
            animation: fadeIn 0.5s ease-in;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .tooltip {
            position: relative;
        }
        
        .tooltip:hover .tooltip-text {
            visibility: visible;
            opacity: 1;
        }
        
        .tooltip-text {
            visibility: hidden;
            width: 120px;
            background-color: var(--dark);
            color: #fff;
            text-align: center;
            border-radius: 6px;
            padding: 5px;
            position: absolute;
            z-index: 1;
            bottom: 125%;
            left: 50%;
            margin-left: -60px;
            opacity: 0;
            transition: opacity 0.3s;
        }
    </style>
</head>
<body class="bg-gray-50">
    <div class="container mx-auto px-4 py-8 max-w-7xl fade-in">
        <div class="flex justify-between items-center mb-8">
            <div>
                <h1 class="text-3xl font-bold text-gray-800">布行财务管理系统</h1>
                <p class="text-gray-600">高端面料行业专业财务解决方案</p>
            </div>
            <div class="flex items-center">
                <div class="mr-4">
                    <span class="text-sm text-gray-500">当前月份:</span>
                    <span class="font-medium">2025年5月</span>
                </div>
                <button class="btn-primary text-white px-4 py-2 rounded-lg flex items-center">
                    <i class="fas fa-download mr-2"></i> 导出报表 
                </button>
            </div>
        </div>
 
        <div class="bg-white rounded-xl shadow-sm p-6 mb-8">
            <div class="flex justify-between items-center mb-6">
                <h2 class="text-xl font-semibold text-gray-800">月度财务概览</h2>
                <div class="flex space-x-2">
                    <div class="bg-blue-50 text-blue-800 px-3 py-1 rounded-full text-sm">
                        <i class="fas fa-sync-alt mr-1"></i> 实时更新 
                    </div>
                    <div class="bg-green-50 text-green-800 px-3 py-1 rounded-full text-sm">
                        <i class="fas fa-check-circle mr-1"></i> 已验证 
                    </div>
                </div>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-4 gap-4">
                <div class="bg-gradient-to-r from-blue-50 to-indigo-50 p-4 rounded-lg border border-blue-100">
                    <div class="flex justify-between items-start">
                        <div>
                            <p class="text-sm text-blue-600">总收入</p>
                            <h3 class="text-2xl font-bold text-blue-800 mt-1">¥85,420</h3>
                        </div>
                        <div class="bg-blue-100 text-blue-600 p-2 rounded-full">
                            <i class="fas fa-wallet"></i>
                        </div>
                    </div>
                    <p class="text-xs text-blue-500 mt-2"><i class="fas fa-arrow-up mr-1"></i> 12.5% 较上月</p>
                </div>
                
                <div class="bg-gradient-to-r from-red-50 to-pink-50 p-4 rounded-lg border border-red-100">
                    <div class="flex justify-between items-start">
                        <div>
                            <p class="text-sm text-red-600">总支出</p>
                            <h3 class="text-2xl font-bold text-red-800 mt-1">¥42,150</h3>
                        </div>
                        <div class="bg-red-100 text-red-600 p-2 rounded-full">
                            <i class="fas fa-receipt"></i>
                        </div>
                    </div>
                    <p class="text-xs text-red-500 mt-2"><i class="fas fa-arrow-down mr-1"></i> 5.3% 较上月</p>
                </div>
                
                <div class="bg-gradient-to-r from-purple-50 to-indigo-50 p-4 rounded-lg border border-purple-100">
                    <div class="flex justify-between items-start">
                        <div>
                            <p class="text-sm text-purple-600">客户欠款</p>
                            <h3 class="text-2xl font-bold text-purple-800 mt-1">¥23,750</h3>
                        </div>
                        <div class="bg-purple-100 text-purple-600 p-2 rounded-full">
                            <i class="fas fa-hand-holding-usd"></i>
                        </div>
                    </div>
                    <p class="text-xs text-purple-500 mt-2"><i class="fas fa-info-circle mr-1"></i> 5位客户未结清</p>
                </div>
                
                <div class="bg-gradient-to-r from-teal-50 to-emerald-50 p-4 rounded-lg border border-teal-100">
                    <div class="flex justify-between items-start">
                        <div>
                            <p class="text-sm text-teal-600">净利润</p>
                            <h3 class="text-2xl font-bold text-teal-800 mt-1">¥43,270</h3>
                        </div>
                        <div class="bg-teal-100 text-teal-600 p-2 rounded-full">
                            <i class="fas fa-chart-line"></i>
                        </div>
                    </div>
                    <p class="text-xs text-teal-500 mt-2"><i class="fas fa-arrow-up mr-1"></i> 18.2% 较上月</p>
                </div>
            </div>
        </div>
 
        <div class="mb-6">
            <div class="flex border-b border-gray-200">
                <button class="tab-active px-4 py-2 text-sm font-medium">财务总览</button>
                <button class="px-4 py-2 text-sm font-medium text-gray-500 hover:text-gray-700">图表分析</button>
                <button class="px-4 py-2 text-sm font-medium text-gray-500 hover:text-gray-700">年度报表</button>
            </div>
        </div>
 
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-6 mb-8">
            <div class="lg:col-span-2">
                <div class="bg-white rounded-xl shadow-sm overflow-hidden">
                    <div class="table-header px-6 py-4 flex justify-between items-center">
                        <h3 class="text-lg font-semibold text-white">每日收支记录</h3>
                        <button class="btn-secondary text-white px-3 py-1 rounded-lg text-sm flex items-center">
                            <i class="fas fa-plus mr-1"></i> 新增记录 
                        </button>
                    </div>
                    <div class="overflow-x-auto">
                        <table class="min-w-full divide-y divide-gray-200">
                            <thead class="bg-gray-50">
                                <tr>
                                    <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">日期</th>
                                    <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">收入</th>
                                    <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">支出</th>
                                    <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">备注</th>
                                    <th scope="col" class="px-6 py-3 text-right text-xs font-medium text-gray-500 uppercase tracking-wider">操作</th>
                                </tr>
                            </thead>
                            <tbody class="bg-white divide-y divide-gray-200">
                                <tr class="highlight-row">
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="date" class="input-field border border-gray-200 px-2 py-1 w-32" value="2025-05-01">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="number" class="input-field border border-gray-200 px-2 py-1 w-24" value="12500">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="number" class="input-field border border-gray-200 px-2 py-1 w-24" value="3200">
                                    </td>
                                    <td class="px-6 py-4">
                                        <input type="text" class="input-field border border-gray-200 px-2 py-1 w-full" placeholder="备注信息" value="丝绸面料销售">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap text-right">
                                        <button class="text-blue-600 hover:text-blue-800 mr-2 tooltip">
                                            <i class="fas fa-save"></i>
                                            <span class="tooltip-text">保存修改</span>
                                        </button>
                                        <button class="text-red-600 hover:text-red-800 tooltip">
                                            <i class="fas fa-trash"></i>
                                            <span class="tooltip-text">删除记录</span>
                                        </button>
                                    </td>
                                </tr>
                                <tr class="highlight-row">
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="date" class="input-field border border-gray-200 px-2 py-1 w-32" value="2025-05-03">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="number" class="input-field border border-gray-200 px-2 py-1 w-24" value="8500">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="number" class="input-field border border-gray-200 px-2 py-1 w-24" value="5800">
                                    </td>
                                    <td class="px-6 py-4">
                                        <input type="text" class="input-field border border-gray-200 px-2 py-1 w-full" placeholder="备注信息" value="亚麻面料采购">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap text-right">
                                        <button class="text-blue-600 hover:text-blue-800 mr-2">
                                            <i class="fas fa-save"></i>
                                        </button>
                                        <button class="text-red-600 hover:text-red-800">
                                            <i class="fas fa-trash"></i>
                                        </button>
                                    </td>
                                </tr>
                                <tr class="highlight-row">
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="date" class="input-field border border-gray-200 px-2 py-1 w-32" value="2025-05-05">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="number" class="input-field border border-gray-200 px-2 py-1 w-24" value="0">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="number" class="input-field border border-gray-200 px-2 py-1 w-24" value="4200">
                                    </td>
                                    <td class="px-6 py-4">
                                        <input type="text" class="input-field border border-gray-200 px-2 py-1 w-full" placeholder="备注信息" value="店铺租金">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap text-right">
                                        <button class="text-blue-600 hover:text-blue-800 mr-2">
                                            <i class="fas fa-save"></i>
                                        </button>
                                        <button class="text-red-600 hover:text-red-800">
                                            <i class="fas fa-trash"></i>
                                        </button>
                                    </td>
                                </tr>
                                <tr class="highlight-row">
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="date" class="input-field border border-gray-200 px-2 py-1 w-32" value="2025-05-08">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="number" class="input-field border border-gray-200 px-2 py-1 w-24" value="18700">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="number" class="input-field border border-gray-200 px-2 py-1 w-24" value="0">
                                    </td>
                                    <td class="px-6 py-4">
                                        <input type="text" class="input-field border border-gray-200 px-2 py-1 w-full" placeholder="备注信息" value="高端定制订单">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap text-right">
                                        <button class="text-blue-600 hover:text-blue-800 mr-2">
                                            <i class="fas fa-save"></i>
                                        </button>
                                        <button class="text-red-600 hover:text-red-800">
                                            <i class="fas fa-trash"></i>
                                        </button>
                                    </td>
                                </tr>
                                <tr class="highlight-row">
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="date" class="input-field border border-gray-200 px-2 py-1 w-32" value="">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="number" class="input-field border border-gray-200 px-2 py-1 w-24" placeholder="0">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="number" class="input-field border border-gray-200 px-2 py-1 w-24" placeholder="0">
                                    </td>
                                    <td class="px-6 py-4">
                                        <input type="text" class="input-field border border-gray-200 px-2 py-1 w-full" placeholder="新增记录">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap text-right">
                                        <button class="text-green-600 hover:text-green-800">
                                            <i class="fas fa-plus-circle"></i> 添加 
                                        </button>
                                    </td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                </div>
            </div>
 
            <div>
                <div class="bg-white rounded-xl shadow-sm overflow-hidden mb-6">
                    <div class="table-header px-6 py-4">
                        <h3 class="text-lg font-semibold text-white">客户欠款管理</h3>
                    </div>
                    <div class="overflow-x-auto">
                        <table class="min-w-full divide-y divide-gray-200">
                            <thead class="bg-gray-50">
                                <tr>
                                    <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">客户名称</th>
                                    <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">欠款金额</th>
                                    <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">操作</th>
                                </tr>
                            </thead>
                            <tbody class="bg-white divide-y divide-gray-200">
                                <tr class="highlight-row">
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="text" class="input-field border border-gray-200 px-2 py-1 w-full" value="杭州时尚服饰">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="number" class="input-field border border-gray-200 px-2 py-1 w-24" value="8500">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <button class="text-purple-600 hover:text-purple-800 text-sm">
                                            <i class="fas fa-hand-holding-usd mr-1"></i> 还款 
                                        </button>
                                    </td>
                                </tr>
                                <tr class="highlight-row">
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="text" class="input-field border border-gray-200 px-2 py-1 w-full" value="上海丝绸设计">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="number" class="input-field border border-gray-200 px-2 py-1 w-24" value="12500">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <button class="text-purple-600 hover:text-purple-800 text-sm">
                                            <i class="fas fa-hand-holding-usd mr-1"></i> 还款 
                                        </button>
                                    </td>
                                </tr>
                                <tr class="highlight-row">
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="text" class="input-field border border-gray-200 px-2 py-1 w-full" value="南京纺织厂">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="number" class="input-field border border-gray-200 px-2 py-1 w-24" value="2750">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <button class="text-purple-600 hover:text-purple-800 text-sm">
                                            <i class="fas fa-hand-holding-usd mr-1"></i> 还款 
                                        </button>
                                    </td>
                                </tr>
                                <tr class="highlight-row">
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="text" class="input-field border border-gray-200 px-2 py-1 w-full" placeholder="新增客户">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="number" class="input-field border border-gray-200 px-2 py-1 w-24" placeholder="0">
                                    </td>
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <button class="text-green-600 hover:text-green-800 text-sm">
                                            <i class="fas fa-plus-circle mr-1"></i> 添加 
                                        </button>
                                    </td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                </div>
 
                <div class="bg-white rounded-xl shadow-sm overflow-hidden">
                    <div class="table-header px-6 py-4">
                        <h3 class="text-lg font-semibold text-white">客户还款记录</h3>
                    </div>
                    <div class="overflow-x-auto">
                        <table class="min-w-full divide-y divide-gray-200">
                            <thead class="bg-gray-50">
                                <tr>
                                    <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">日期</th>
                                    <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">客户</th>
                                    <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">还款金额</th>
                                </tr>
                            </thead>
                            <tbody class="bg-white divide-y divide-gray-200">
                                <tr class="highlight-row">
                                    <td class="px-6 py-4 whitespace-nowrap">2025-05-02</td>
                                    <td class="px-6 py-4">杭州时尚服饰</td>
                                    <td class="px-6 py-4 text-green-600 font-medium">¥3,200</td>
                                </tr>
                                <tr class="highlight-row">
                                    <td class="px-6 py-4 whitespace-nowrap">2025-05-04</td>
                                    <td class="px-6 py-4">上海丝绸设计</td>
                                    <td class="px-6 py-4 text-green-600 font-medium">¥5,000</td>
                                </tr>
                                <tr class="highlight-row">
                                    <td class="px-6 py-4 whitespace-nowrap">2025-05-07</td>
                                    <td class="px-6 py-4">南京纺织厂</td>
                                    <td class="px-6 py-4 text-green-600 font-medium">¥2,750</td>
                                </tr>
                                <tr class="highlight-row">
                                    <td class="px-6 py-4 whitespace-nowrap">
                                        <input type="date" class="input-field border border-gray-200 px-2 py-1 w-32" placeholder="选择日期">
                                    </td>
                                    <td class="px-6 py-4">
                                        <select class="input-field border border-gray-200 px-2 py-1 w-full">
                                            <option>选择客户</option>
                                            <option>杭州时尚服饰</option>
                                            <option>上海丝绸设计</option>
                                            <option>南京纺织厂</option>
                                        </select>
                                    </td>
                                    <td class="px-6 py-4">
                                        <input type="number" class="input-field border border-gray-200 px-2 py-1 w-24" placeholder="金额">
                                        <button class="ml-2 text-green-600 hover:text-green-800">
                                            <i class="fas fa-check"></i>
                                        </button>
                                    </td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                </div>
            </div>
        </div>
 
        <div class="bg-white rounded-xl shadow-sm overflow-hidden">
            <div class="table-header px-6 py-4 flex justify-between items-center">
                <h3 class="text-lg font-semibold text-white">月度利润计算表</h3>
                <div class="flex items-center">
                    <span class="text-white text-sm mr-3">利润率: 50.6%</span>
                    <span class="bg-white bg-opacity-20 px-2 py-1 rounded text-xs">优秀</span>
                </div>
            </div>
            <div class="overflow-x-auto">
                <table class="min-w-full divide-y divide-gray-200">
                    <thead class="bg-gray-50">
                        <tr>
                            <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">项目</th>
                            <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">金额</th>
                            <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">占比</th>
                            <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">趋势</th>
                        </tr>
                    </thead>
                    <tbody class="bg-white divide-y divide-gray-200">
                        <tr class="highlight-row">
                            <td class="px-6 py-4 whitespace-nowrap font-medium">总收入</td>
                            <td class="px-6 py-4 whitespace-nowrap">¥85,420</td>
                            <td class="px-6 py-4 whitespace-nowrap">100%</td>
                            <td class="px-6 py-4 whitespace-nowrap">
                                <span class="text-green-500"><i class="fas fa-arrow-up mr-1"></i>12.5%</span>
                            </td>
                        </tr>
                        <tr class="highlight-row">
                            <td class="px-6 py-4 whitespace-nowrap font-medium">总支出</td>
                            <td class="px-6 py-4 whitespace-nowrap">¥42,150</td>
                            <td class="px-6 py-4 whitespace-nowrap">49.4%</td>
                            <td class="px-6 py-4 whitespace-nowrap">
                                <span class="text-red-500"><i class="fas fa-arrow-down mr-1"></i>5.3%</span>
                            </td>
                        </tr>
                        <tr class="highlight-row bg-gray-50">
                            <td class="px-6 py-4 whitespace-nowrap font-bold">净利润</td>
                            <td class="px-6 py-4 whitespace-nowrap font-bold text-blue-600">¥43,270</td>
                            <td class="px-6 py-4 whitespace-nowrap font-bold">50.6%</td>
                            <td class="px-6 py-4 whitespace-nowrap">
                                <span class="text-green-500 font-bold"><i class="fas fa-arrow-up mr-1"></i>18.2%</span>
                            </td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </div>
 
        <div class="mt-8 text-center text-sm text-gray-500">
            <p>© 2025 布行财务管理系统 | 高端面料行业专业解决方案</p>
            <p class="mt-1">数据最后更新时间: 2025-05-09 15:30:45</p>
        </div>
    </div>
 
    <script>
        // 这里可以添加交互逻辑 
        document.addEventListener('DOMContentLoaded',  function() {
            // 简单的交互效果 
            const rows = document.querySelectorAll('.highlight-row'); 
            rows.forEach(row  => {
                row.addEventListener('mouseenter',  function() {
                    this.style.transform  = 'translateX(2px)';
                });
                row.addEventListener('mouseleave',  function() {
                    this.style.transform  = 'translateX(0)';
                });
            });
            
            // 标签切换效果 
            const tabs = document.querySelectorAll('.flex.border-b  button');
            tabs.forEach(tab  => {
                tab.addEventListener('click',  function() {
                    tabs.forEach(t  => t.classList.remove('tab-active')); 
                    this.classList.add('tab-active'); 
                });
            });
        });
    </script>
</body>
</html>
